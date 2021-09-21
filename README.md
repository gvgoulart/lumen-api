<h1>Instruções para instalação:</h1>

Após a clonagem do repositório, fazer a instalação do composer na raíz do projeto:
```
composer install
```
Fazer a configuração do arquivo .env copiando o arquivo .env.example:
```
cp .env.example .env
```
Após a configuração do banco de dados em .env, executar as migrations:
```
php artisan migrate:fresh
```

Para geração das chaves de uso do passport:
```
php artisan passport:install
```

Caso a instalação do passport de erro siga os seguintes passos:
```
php artisan cache:clear
```

```
php artisan config:clear
```

```
composer dump-autoload
```
E se mesmo assim não der certo
![image](https://user-images.githubusercontent.com/71338619/130554717-6dd846c5-a48e-494a-8d15-a9ff5ec51bdd.png)

Exclua a linha 28
```
php artisan passport:install
```
E insira ela novamente


# Lumen PHP Framework

[![Build Status](https://travis-ci.org/laravel/lumen-framework.svg)](https://travis-ci.org/laravel/lumen-framework)
[![Total Downloads](https://img.shields.io/packagist/dt/laravel/framework)](https://packagist.org/packages/laravel/lumen-framework)
[![Latest Stable Version](https://img.shields.io/packagist/v/laravel/framework)](https://packagist.org/packages/laravel/lumen-framework)
[![License](https://img.shields.io/packagist/l/laravel/framework)](https://packagist.org/packages/laravel/lumen-framework)

Laravel Lumen is a stunningly fast PHP micro-framework for building web applications with expressive, elegant syntax. We believe development must be an enjoyable, creative experience to be truly fulfilling. Lumen attempts to take the pain out of development by easing common tasks used in the majority of web projects, such as routing, database abstraction, queueing, and caching.

## Official Documentation

Documentation for the framework can be found on the [Lumen website](https://lumen.laravel.com/docs).

## Contributing

Thank you for considering contributing to Lumen! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Security Vulnerabilities

If you discover a security vulnerability within Lumen, please send an e-mail to Taylor Otwell at taylor@laravel.com. All security vulnerabilities will be promptly addressed.

## License

The Lumen framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
