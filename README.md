Advanced Paypal IPN Documentation 

To create a module, simply create a new text .php file with the name of your choice.
Then create a function with the name of your choice and have what you want run inside of it.
You can then load the module within config.php.
There are many different features you can add to your module.
An example of a feature is the mysql connection feature, fill in the details on the config.php and then simply write:

if (!$link) {
    die('Could not connect: ' . mysql_error());
}

This will then check for a valid connection.
Remember to add mysql_close after all of your queries.

When creating a variable, it is highly recommended that you include the lib.php file using the following code;
include(lib.php);
This will include the entire paypal IPN variable library.

Any PHP function can be run at all.

IPN

Email Feature in config.php.

Everytime someone purchases something and it communicates with the IPN system, it will send an email if its successful, you can edit this email in config.php.
Feel free to use any of these variables within your config.php, they are all included in the includes file which will be left untouched.

https://cms.paypal.com/us/cgi-bin/?cmd=_render-content&content_ID=developer/e_howto_admin_IPNReference
format : $variablename

Paypal Library

We have included a paypal library with every single ipn variable.
To include it write in your php script:
include("lib.php");
To include the configuration settings write:
include("config.php");
More updates will be coming every now and then.
Please email me suggestions or bugs at olimoli123@hotmail.com


