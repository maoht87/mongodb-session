Laravel MongoDB Session
=======================

A MongoDB session driver for Laravel 4, inspired by LMongo. For more information about Sessions, check http://laravel.com/docs/eloquent.

Installation
------------

Make sure you have [omt\mongodb](https://github.com/maoht87/MongoDB) installed before you continue.

Install using composer:

    composer require omt/mongodb-session

Add the session service provider in `app/config/app.php`:

    'OMT\Mongodb\Session\SessionServiceProvider',

Change the session driver in `app/config/session.php` to mongodb:

    'driver' => 'mongodb',

*Optional*: change the connection to a connection using the mongodb driver from `app/config/database.php`:

	'connection' => 'mongodb',
