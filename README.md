- Pour utiliser des bibliothéques externe, on installe composer
# composer init

- Pour faire des tests unitaires, on installe phpunit
# composer require --dev phpunit/phpunit

- Pour lancer server interne
# php -S localhost:8000 -d display_error=1 -t public

- Lorsque l'on ajout un autoloader
    "autoload": {
        "psr-4": {
            "Framework\\": "src/Framework"
        }
    }
- il ne faut pas oublier de faire
# composer dump-autoload

- Pour lancer des tests avec phpunit :
# ./vendor/bin/phpunit tests/Framework/Apptest.php