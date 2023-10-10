## Laravel with Filament and ReactJS


- Laravel app build with Filament Admin components and ReactJS for the front-end views
- Laravel Docs current build v10 [Doc link](https://laravel.com)
- Filament Docs [Doc link](https://filamentphp.com/docs)
- Tailwind CSS [Tailwind CSS Doc link](https://tailwindcss.com/)
- Tailwind Components (Components Doc link)[https://tailwindui.com/?ref=top]

### Build Structure

- Laravel 
- Filament
- Tailwind CSS
- Sass compiler Webpack or Gulp, come in later
- ReactJS
- Docker setup will come in later


### Installation

- Install Laravel
- Install Filament: Read their Docs
    - `composer require filament/filament:"^3.0-stable" -W`
    - Install the panel with command `php artisan filament:install --panels`
    - connect to DB and run    `php artisan migrate`
    - create a user for Filament admin login `php artisan make:filament-user` , fill in the details
    - generate storage link `php artisan storage:link`
    - create *Model Post* with migration `php artisan make:model Post -m`
    - create *Model Category* with migration `php artisan make:model Category -m`
    - create *Model CategoryPost* with migration `php artisan make:model CategoryPost -m`
    - create admin dashboard resources/panels [Doc link here](https://filamentphp.com/docs/3.x/panels/resources/getting-started)
    - using package Doctrine/dbal so we can install complex dashboard panels based on the DB schema ( used for dedicated create,edit,update) `composer require doctrine/dbal --dev`
    - create admin dashboard panel `php artisan make:filament-resource Category --simple --generate`. Simple flag is used if the record is simple. Read docs about this. [Doc link here](https://filamentphp.com/docs/3.x/panels/resources/getting-started)
    - create admin dashboard for Post with view. `php artisan make:filament-resource Post --view --generate`


### About Laravel 

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

### Tutorial Source

- [Part 1](https://www.youtube.com/watch?v=iVThaG_sAt0&list=PLl9U9DCkJjWnNDf_8mpNAnEeqIiljwDoE&index=103&t=1584s)
- [Part 2](https://www.youtube.com/watch?v=2ZkePm2D6SI&list=PLl9U9DCkJjWnNDf_8mpNAnEeqIiljwDoE&index=105&t=18s)

### Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.


### License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
