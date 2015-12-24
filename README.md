#Codeigniter Database

Use the Session Library separately from CodeIgniter 3.

## Installation

###With Composer
```json
"require": {
    // ...
    "evolution/ci_session":  "dev-master"
}
```

###Without Composer

You can also download it from Github, but no autoloader is provided so you'll need to register it with your own PSR-0 compatible autoloader.

#Usage
```php
<?php
use Evolution\CodeIgniterSession\CI_Session as Session;
$config['driver'] = 'files';
$config['cookie_name'] = 'ci_session';
$config['expiration'] = 7200;
$config['save_path'] = NULL;
$config['match_ip'] = FALSE;
$config['time_to_update'] = 300;
$config['regenerate_destroy'] = FALSE;
$config['cookie_prefix']	= '';
$config['cookie_domain']	= '';
$config['cookie_path']		= '/';
$config['cookie_secure']	= FALSE;
$config['cookie_httponly'] 	= FALSE;

$session = new CI_Session($config);
```
For more information visit <a href="http://www.codeigniter.com/userguide3/libraries/sessions.html">CodeIgniter user guide</a>.
