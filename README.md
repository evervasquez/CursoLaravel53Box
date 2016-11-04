# Configuración del entorno de trabajo

### Sistema operativo
Ubuntu 14.04.5

### Software instalado
* PHP 7.0.12-1
* nginx version: nginx/1.4.6
* php-fpm7.0
* mysql  Ver 14.14 Distrib 5.5.52

### Add Box
```
$ vagrant box add sonico999/devcode
$ git clone git@github.com:evervasquez/CursoLaravel53Box.git FundamentosLaravel53
$ vagrant up --provider virtualbox
```

### Conexión a la base de datos (mysql)
* Host = 127.0.0.1
* Port = 33060
* User = root
* Pass =


### Agregar a hosts
```
192.168.1.241 reddit.dev
```

### Crear proyecto de laravel 
```
$ composer create-project --prefer-dist laravel/laravel reddit-devcode

```

### IP
192.168.1.241
