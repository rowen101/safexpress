<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**
- **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
- **[Lendio](https://lendio.com)**

## laravel-datatables
-Laravel Version Compatibility

| Laravel | Package  |
|:--------|:---------|
| 4.2.x   | 3.x      |
| 5.0.x   | 6.x      |
| 5.1.x   | 6.x      |
| 5.2.x   | 6.x      |
| 5.3.x   | 6.x      |
| 5.4.x   | 7.x, 8.x |
| 5.5.x   | 8.x      |
| 5.6.x   | 8.x      |
| 5.7.x   | 8.x      |
| 5.8.x   | 9.x      |
| 6.x.x   | 9.x      |
| 7.x.x   | 9.x      |
| 8.x.x   | 9.x      |
| 9.x.x   | 10.x     |
| 10.x.x  | 10.x     |

## Quick Installation

```bash
composer require yajra/laravel-datatables-oracle:"^10.0"
```

#### Service Provider & Facade (Optional on Laravel 5.5+)

Register provider and facade on your `config/app.php` file.
```php
'providers' => [
    ...,
    Yajra\DataTables\DataTablesServiceProvider::class,
]

'aliases' => [
    ...,
    'DataTables' => Yajra\DataTables\Facades\DataTables::class,
]
```

#### Configuration (Optional)

```bash
php artisan vendor:publish --provider="Yajra\DataTables\DataTablesServiceProvider"
```

And that's it! Start building out some awesome DataTables!

## Debugging Mode

To enable debugging mode, just set `APP_DEBUG=true` and the package will include the queries and inputs used when processing the table.

**IMPORTANT:** Please make sure that APP_DEBUG is set to false when your app is on production.

## PHP ARTISAN SERVE BUG

Please avoid using `php artisan serve` when developing with the package.
There are known bugs when using this where Laravel randomly returns a redirect and 401 (Unauthorized) if the route requires authentication and a 404 NotFoundHttpException on valid routes.

It is advised to use [Homestead](https://laravel.com/docs/5.4/homestead) or [Valet](https://laravel.com/docs/5.4/valet) when working with the package.

## Contributing

Please see [CONTRIBUTING](https://github.com/yajra/laravel-datatables/blob/master/.github/CONTRIBUTING.md) for details.
## Breadcrumbs
```bash
composer require diglactic/laravel-breadcrumbs
```
## Intervention image
```bash
composer require intervention/image
```
## build docker 
```bash
docker-compose up --build 
```
## run docker or stop
```bash
docker-compose up
docker-compose down
```
## view logs container name
```bash
docker logs containername
```
## docker in windows 10 access file
winpty docker exec -it containername //bin//sh
docker exec -it Safexpress /bin/sh

To access your Laravel application : http://localhost:8000
To access the PhpMyAdmin console: http://localhost:8081
The MySQL Database is using the port: 3306
