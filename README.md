# drupal-gitlab-unit-test

[![Build Status](https://travis-ci.org/vigetlabs/gulp-starter.svg?branch=static-server)](https://travis-ci.org/vigetlabs/gulp-starter)

## About
Gitlab + Gulp : Currently only for Drupal 8 projects. Stay tune....

## Features
* Automated coding standard(Drupal Coding Standards, CSS Linting, JS Linting) check using [coder](https://www.drupal.org/project/coder)
, [eslint](http://eslint.org), [csslint](http://csslint.net). The infrastructure has been setup using gulp](http://gulpjs.com) and
[gitlab].

## Future Roadmap
* Make the directory paths generic for all Drupal projects.
* Update .gitlab-ci.yml correctly
* Add some more unit test and Auto fixer https://github.com/vigetlabs/gulp-starter



## Dependencies
You need npm and composer to use this, please install npm and composer using the steps as per our
OS.
* Composer: https://getcomposer.org/download/
* npm: https://www.npmjs.com/

## Steps to install
Once all the dependencies are installed, follow the steps below

* Clone the repo
* Execute ```npm install -g gulp```
* Execute ```npm install```
* Execute ```composer install```
* Move your Drupal codebase to project directory

## How to use
You can check for coding standards either in your system or use it during a pull request

### Local
* Execute ```gulp``` inside your project to check for coding standards

### Warning
* make sure your node version is update to date or you might face this error
```const path = require('path');
^^^^^
SyntaxError: Use of const in strict mode.
    at Module._compile (module.js:439:25)
    at Object.Module._extensions..js (module.js:474:10)
    at Module.load (module.js:356:32)
    at Function.Module._load (module.js:312:12)
    at Module.require (module.js:364:17)
    at require (module.js:380:17)
    at Object.<anonymous> (D:\project\gulpfile.js:87:16)
    at Module._compile (module.js:456:26)
    at Object.Module._extensions..js (module.js:474:10)
    at Module.load (module.js:356:32)```

* how to update node.js version with NPM
* ```npm install -g n```
* ```n stable```

The n package represents a Node helper, and running the last command upgrades node to the latest stable version.  Instead of using "stable", you could specify a desired version:
example : n 0.8.21
