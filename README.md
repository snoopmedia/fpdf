Generation to PDF for use with Symfony 2
==============================

Uses FPDF 1.7

Setup
-----

Add the following lines to your 'composer.json' file:


        "require": {
                "php": ">=5.3.3",
                "symfony/symfony": "2.1.*",
                .......
                "snoopmedia/fpdf": "*"
         },
        "repositories": [
                {
                    "type": "package",
                    "package": {
                        "name": "snoopmedia/fpdf",
                        "version": "1.0.1",
                        "dist": {
                            "url": "https://github.com/snoopmedia/fpdf/archive/master.zip",
                            "type": "zip"
                        },
                        "autoload": {
                            "psr-0": { "Snoopmedia": "" }
                        },
                        "target-dir": "Snoopmedia"
                    }
                }
            ],


Now run `php composer.phar  update` or `php composer.phar install`.

Usage
--------

        $pdf = new \PDF;

Sources
---------
[FPDF](http://www.fpdf.org/)

