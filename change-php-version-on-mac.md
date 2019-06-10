`sudo nano ~/.bash_profile`

`export XAMPP_HOME=/Applications/XAMPP`

`export PATH=${XAMPP_HOME}/bin:${PATH}`

`export PATH`

Load the changes with this (won't be needed next time you open a shell session):

`source ~/.bash_profile`
Confirm:

$ which php
/Applications/XAMPP/bin/php
