# [Sage](https://roots.io/sage/)

Sage is a WordPress starter theme with a modern development workflow.

## Features

* Sass for stylesheets
* Modern JavaScript
* [Laravel Mix](https://github.com/JeffreyWay/laravel-mix) for compiling assets and concatenating and minifying files
* [Browsersync](http://www.browsersync.io/) for synchronized browser testing
* [Blade](https://laravel.com/docs/5.8/blade) as a templating engine
* [Tailwind CSS](https://tailwindcss.com/) Utility based CSS framework
* [Vue](https://vuejs.org/v2/guide/) JS framework

## Requirements

Make sure all dependencies have been installed before moving on:

* [WordPress](https://wordpress.org/) >= 5.2
* [PHP](https://secure.php.net/manual/en/install.php) >= 7.1.3 (with [`php-mbstring`](https://secure.php.net/manual/en/book.mbstring.php) enabled)
* [Composer](https://getcomposer.org/download/)
* [Node.js](http://nodejs.org/) >= 8.0.0
* [Yarn](https://yarnpkg.com/en/docs/install)

## Theme installation

This readme assumes you are familiar with [Sage](https://github.com/roots/sage) and [Bedrock](https://github.com/roots/bedrock) structure for Wordpress. If not, head over to [https://roots.io/](https://roots.io/) to learn more.

```sh
# @ app/themes/ or wp-content/themes/
$ git clone git@github.com:alithedeveloper/sage-vue-tailwind.git
$ cd sage-vue-tailwind
$ composer install
$ yarn
$ yarn dev / production / watch
```


## Theme structure

```sh
themes/your-theme-name/   # → Root of your Sage based theme
├── composer.json         # → Autoloading for `app/` files
├── composer.lock         # → Composer lock file (never edit)
├── dist/                 # → Built theme assets (never edit)
├── functions.php         # → Composer autoloader, Acorn bootloader
├── index.php             # → Never manually edit
├── node_modules/         # → Node.js packages (never edit)
├── package.json          # → Node.js dependencies and scripts
├── screenshot.png        # → Theme screenshot for WP admin
├── style.css             # → Theme meta information
├── app/                  # → Theme PHP
│   ├── Composers/        # → View composers
│   ├── Providers/        # → Service providers
│   ├── admin.php         # → Theme customizer setup
│   ├── filters.php       # → Theme filters
│   ├── helpers.php       # → Helper functions
│   └── setup.php         # → Theme setup
├── config/               # → Config files
│   ├── app.php           # → Application configuration
│   ├── assets.php        # → Asset configuration
│   ├── filesystems.php   # → Filesystems configuration
│   ├── logging.php       # → Logging configuration
│   └── view.php          # → View configuration
├── dist/                 # → Built theme assets (never edit)
├── resources/            # → Theme assets and templates
│   ├── assets/           # → Front-end assets
│   │   ├── fonts/        # → Theme fonts
│   │   ├── images/       # → Theme images
│   │   ├── scripts/      # → Theme JS
│   │   └── styles/       # → Theme stylesheets
│   └── views/            # → Theme templates
│       ├── layouts/      # → Base templates
│       └── partials/     # → Partial templates
├── storage/              # → Storage location for cache (never edit)
└── vendor/               # → Composer packages (never edit)
```

## Theme setup

Edit `app/setup.php` to enable or disable theme features, setup navigation menus, post thumbnail sizes, and sidebars.

## Theme development

* Run `yarn` from the theme directory to install dependencies
* Update `webpack.mix.js` with your local dev URL

### Build commands

* `yarn start` — Compile assets when file changes are made, start Browsersync session
* `yarn build` — Compile and optimize the files in your assets directory
* `yarn build:production` — Compile assets for production

## Documentation

* [Sage documentation](https://roots.io/sage/docs/)




