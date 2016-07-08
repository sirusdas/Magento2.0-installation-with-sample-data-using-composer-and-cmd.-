Easiest steps to install Magento in one chance.
Follow this steps:
Required: 
Xampp installed.
Download the Magento from the official website with sample data.
Download the composer.
Enable the shell option while installing composer.
Now follow me. 
Open php.ini file and do some tweaks.
Details in the folder of magento setup.
Done then follow me
Go to the magento and righ click on the composer.json and then composer install if all fine then composer update.
Done then in the same cmd type this command:
php bin/magento setup:upgrade
fine
now 
this
if you get a php fatal error or something then do this in the php.ini file
change the memory to 256.
Make sure you follow each steps correctly.
And BE HAPPY :D

Create db from CMD:
php bin/magento setup:install --base-url=http://localhost:8080/magento2/ --db-host=localhost --db-name= magento2 --db-user=root --db-password="root" --admin-firstname=sirus --admin-lastname=das --admin-email=abc@gmail.com --admin-user=sirusdas --admin-password=admin123 --language=en_US --currency=INR --timezone=Asia/Kolkata --use-rewrites=1


Uninstall Magento from CMD:
php bin/magento setup:uninstall

Upgrade Magento:
php bin/magento setup:upgrade

admin
admin123
admin_c71a0w
admin_z2pqf4
links to follow
http://devdocs.magento.com/guides/v2.0/install-gde/install/cli/install-cli-subcommands.html
http://devdocs.magento.com/guides/v2.0/install-gde/install/cli/install-cli-subcommands-enable.html#instgde-cli-subcommands-enable-modules
http://devdocs.magento.com/guides/v2.0/install-gde/install/cli/install-cli-sample-data.html
During installation, Reflection Exception error

http://devdocs.magento.com/guides/v2.0/install-gde/trouble/tshoot_wrong-mysql.html
Magento2 Installation with Sample data Error - 0.42.0-beta7 #1033 

https://github.com/magento/magento2/issues/1033
Fatal Error: Allowed Memory Size of 134217728 Bytes Exhausted (CodeIgniter + XML-RPC)
http://stackoverflow.com/questions/561066/fatal-error-allowed-memory-size-of-134217728-bytes-exhausted-codeigniter-xml



MYSQL
The headache was to change my password from null to something
Follow this:
Open xammp and then click the shell or just google the directory where your mysql.exe file is installed and open cmd in that directory.
Now:
Type this mysql –u yourusername –p “”
Hit enter
It will ask for passoword:
Press enter if its null.
Good now 
Change the passoword by tying this code
SET PASSWORD FOR 'jeffrey'@'localhost' = PASSWORD('mypass');
Link: http://dev.mysql.com/doc/refman/5.7/en/set-password.html
If didn’t work do check this link:
http://stackoverflow.com/questions/8463350/how-can-i-switch-to-another-user-in-mysql-via-cmd

Sample data details link:
http://devdocs.magento.com/guides/v2.0/install-gde/install/sample-data-after-magento.html
Install Magento Software from CMD link:
http://devdocs.magento.com/guides/v2.0/install-gde/install/cli/install-cli-install.html#install-cli-example

Time zone details link:
http://php.net/manual/en/timezones.indian.php

php.ini
extension=php_intl.dll
memory_limit=328M
max_input_time=300
max_execution_time=18000
zlib.output_compression=On
session.auto_start=Off
suhosin.session.cryptua = Off




