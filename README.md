# Flickerleap mess detector

This project contains a ruleset to be used with phpmd https://github.com/phpmd/phpmd

## Installation

```bash
$ composer require phpmd/phpmd flickerleap/phpmd
```

## Usage

```bash
$ vendor/bin/phpmd path/to/src text vendor/flickerleap/phpmd/ruleset.xml
```

## Rules
- All phpmd rules
- Excluded static usage of classes due to laravels fantastic service container https://laravel.com/docs/5.6/facades
- Excluded some short variable names such as $to in a mailable
- Excluded all unused parameters due to common usage of $request in controller functions
