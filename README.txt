CONTENTS OF THIS FILE
---------------------
   
 * Introduction
 * Requirements
 * Installation
 * Configuration
 * Instructions
 * Maintainers
 
 
INTRODUCTION
------------
The Site Debug module is used for debugging custom Drupal Module code.  

It involves dumping data to a debug function called sdb() and seeing that dumped data in a text file inside the module called debug.txt.


REQUIREMENTS
------------
There are no external module requirements to use this module.


INSTALLATION
------------
* Install as you would normally install a contributed Drupal module. 
  See: https://drupal.org/documentation/install/modules-themes/modules-7 for further information.
  

CONFIGURATION
-------------
There is no configuration to use this module.


INSTRUCTIONS
------------
Simply add the following function call to your custom module code and then run the code, then check the debug.txt file to see the data.  When finished, select all and delete and begin again.
sdb($variable_or_array_or_object);

EXAMPLES:
sdb($name);
--
sdb('$name = ' . $name);
--
sdb('$day_array');
sdb($day_array);
--
sdb('$day_object');
sdb($day_object);


MAINTAINERS
-----------
* Ray James (rayjames) - https://www.drupal.org/u/rayjames