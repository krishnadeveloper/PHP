## Setps are below install composer globally on mac

1. Open a terminal
2. Run this command shown below to download Composer. This will create a Phar (PHP Archive) file called 
   `curl -sS https://getcomposer.org/installer | php`
3. Now we move composer.phar file to a directory `sudo mv composer.phar /usr/local/bin/`
4. We want to run Composer with having to be root al the time, so we need to change the permissions: `sudo chmod 755 /usr/local/bin/composer.phar`
5. Next, we need to let Bash know where to execute Composer: `nano ~/.bash_profile`
6. Add this line below to bash_profile and save
   `alias composer="php /usr/local/bin/composer.phar"`
7. Run command: `source ~/.bash_profile`

###Now verify the installation

Run command in terminal ; `composer --version`

=============================================

## Quick steps 
 Open termonal
1. `curl -sS https://getcomposer.org/installer | php`

2. `sudo mv composer.phar /usr/local/bin/`
3. Password: "Enter your password"
4. `sudo chmod 755 /usr/local/bin/composer.phar`
5. `nano ~/.bash_profile`
6. Add `alias composer="php /usr/local/bin/composer.phar"` in to opened .bash_profile and save
7. `source ~/.bash_profile`
8. `composer --version`
