# Composer


Installer un nouveau package : 
`composer require <nom-du-package>`

Installer les dépendances à partir de composer.lock avec les versions spécifiées  : 
`composer install`

Met à jour les dépendances et composer.lock avec la dernière versions des packages :
`composer update`

Autoloader les dépendances sur un projet from scratch :
```php
require __DIR__ . '/vendor/autoload.php'
```

Supprimer un package : 
`composer remove <nom-du-package>`