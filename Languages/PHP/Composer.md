# [Composer](https://getcomposer.org/doc/)


**Installer un nouveau package :** 
`composer require <nom-du-package>`

**Installer les dépendances à partir de composer.lock avec les versions spécifiées  :** 
`composer install`

**Met à jour les dépendances et composer.lock avec la dernière versions des packages :**
`composer update`

**Autoloader les dépendances sur un projet from scratch :**
```php
require __DIR__ . '/vendor/autoload.php'
```

**Supprimer un package :** 
`composer remove <nom-du-package>`

**Vider le cache :**
Parfois, un nouveau package que vous venez d'installer via Composer ne semble pas fonctionner du tout. 
Ce problème est généralement causé par une erreur classmap d'une classe de bibliothèque nouvellement installée, ou la version en cache d'une bibliothèque particulière ne correspond pas à celles requises par le code du projet que vous venez de cloner. Dans une telle situation, vous devez mettre à jour l'autoloader PHP en exécutant la commande suivante :
`composer dump-autoload`

**Flags à mettre en production :**
- **--no-interaction (-n)** : Do not ask any interactive question.
- **--no-dev** : Skip installing packages listed in `require-dev`. The autoloader generation skips the `autoload-dev` rules.
- **--optimize-autoloader (-o):** Convert PSR-0/4 autoloading to classmap to get a faster autoloader. This is recommended especially for production, but can take a bit of time to run so it is currently not done by default.