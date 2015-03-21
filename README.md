composer-revision-plugin
========================

Simple composer plugin which generates a class containing the VCS references of all packages

Installation
------------

Just run 

```bash
composer require mcuelenaere/composer-revision-plugin
```

to add this package as a composer dependency to your project.

Usage
-----

All references of the packages you're using in your project can be accessed through the static `ComposerRevisions\Revisions::$byName` variable:

```php
$revisionOfMyProject = ComposerRevisions\Revisions::$byName['foo/my-project'];
$revisionOfMyLibrary = ComposerRevisions\Revisions::$byName['foo/my-library'];
```
