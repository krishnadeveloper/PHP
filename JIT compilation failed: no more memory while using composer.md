Method 1

As a temporary fix, edit your php.ini file (in my case: vi /usr/local/etc/php/7.3/php.ini), disable PHP PCRE JIT compilation by changing:

;pcre.jit=1
to

pcre.jit=0

Method 2

php -d pcre.jit=0 composer.phar

