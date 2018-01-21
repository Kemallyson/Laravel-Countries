# Laravel Countries seeder

This is a laravel repository used to create, migrate and seed countries information to a database. The seeder uses a json source 

## Requirements
* PHP >= 5.6.4
* Laravel 5.4|5.5 (for lararvel 5.5, php 7.0 and above is required)

## Usage
Clone/download the repository. Create a direcory name it data in your database directory
Copy the countries.json file to the data directory


Generate the countries migration file ( using ``php artisan make:migration`` command ), copy the contents of the migrations file in the migrations directory cloned. 

 ``php artisan make:migration create_countries_table --create=countries`` 
 
Generate CountriesTableSeeder file using the artisan command ``php artisan make:seeeder``  command

  ``php artisan make:seeder CountriesTableSeeder``
  
 Generate your model and define the fillable attributes of the table
 
 ```
 protected $fillable = [
        'iso',
        'iso3',
        'fips',
        'country_name',
        'continent',
        'currency_code',
        'currency_name',
        'phone_prefix',
        'postal_code',
        'languages',
        'geonameid'
    ];
  ```
  
  Migrate your table and seed. 
  
  



