SETUP & EXECUTION
=================

Get the framework
=================
* Install the framework:
  * composer require cw_test/behat_framework

Behat setup
===========
* Install Behat:
  * cd vendor/cw_test/behat_framework
  * ./bootstrap.sh
    
Behat configuration
===================
* Inside 'Behat/behat.local.yml', update:
  * the 'base_url' to your local site url
  * the 'drupal_root' value to the path to your local drupal installation.
       

Optional Step
=============
This is only required if you want to run tests on Chrome. 
(By default, Firefox works out-of-the-box.)

1. Download chromedriver from http://chromedriver.storage.googleapis.com/index.html?path=2.17/
2. Save it to /usr/local/bin


Test Execution
==============
1. Open a terminal window.
2. Navigate to [LOCAL DRUPAL INSTALL FOLDER]/Behat
3. To execute the tests, select one of the following options based on the format './run-behat.sh [tag] [profile]':

  - ./run-behat.sh regression firefox
or
  - ./run-behat.sh regression chrome


Test Results
============
The results of all tests will be stored in 
  * [LOCAL DRUPAL INSTALL FOLDER]/Results/Twig_***.html

