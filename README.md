# PHP Database Library
[![Latest Stable Version](https://poser.pugx.org/botfire/botfire/v)](//packagist.org/packages/botfire/botfire)  [![Total Downloads](https://poser.pugx.org/botfire/botfire/downloads)](//packagist.org/packages/botfire/botfire)


### Instal Foxql 
```
composer require webrium/foxql
```

### Add Connection Config
```PHP
use webrium\foxql\DB;

DB::addConfig('main',[
  'driver'=>'mysql' ,
  'db_host'=>'localhost' ,
  'db_host_port'=>3306 ,
  'db_name'=>'test' ,
  'username'=>'root' ,
  'password'=>'1234' ,
  'charset'=>'utf8mb4' ,
  'result_stdClass'=>true
]);
```

> Now it is ready to work :)

## SELECT

```PHP
$user = DB::table('users')->find($user_id);

```