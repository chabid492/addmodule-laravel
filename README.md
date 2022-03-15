Add your service provider in laravel roote folder config/app.php provider array
For example:


	'providers' => [
	     /*
		 * Laravel Framework Service Providers...
		 */

		/*
		 * Package Service Providers...
		 */
		MyVendor\Contactform\ContactFormServiceProvider::class,

	    ],
    

Add these lines in Laravel root folder composer



	  "autoload": {
		"psr-4": {
		    "MyVendor\\Contactform\\": "packages/MyVendor/contactform/src"
		}
	    },


	    "autoload-dev": {
		"psr-4": {
		    "MyVendor\\Contactform\\": "packages/MyVendor/contactform/src"
		}
	    },
