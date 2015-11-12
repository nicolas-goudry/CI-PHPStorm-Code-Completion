# Code Completion for CodeIgniter 3 projects in PHPStorm
##### This repository contains helper files for code completion in phpStorm with CodeIgniter 3.

Original project : https://github.com/topdown/phpStorm-CC-Helpers

CodeIgniter source https://github.com/bcit-ci/CodeIgniter

## Installation instructions

After loading your project, you have two options :
* Set an include path
* Add a content root

**Include path**

Go to `File` > `Settings` > `Project` > `Directories`
Click on `Add Content Root`, select `CI-PHPStorm-Code-Completion` directory and mark it as `Resource Root`

**Content root**

In the project explorer, right click on `External Libraries` then select `Configure PHP Include Paths`. Add the path to the `CI-PHPStorm-Code-Completion` and apply.

**Warning! You have to mark those files as plain text to make code completion works**
* [project]/system/core/Controller.php
* [project]/system/core/Model.php
* [project]/system/database/DB_active_rec.php

Core CodeIgniter Classes should now be available to code completion.

## Make your models available to code completion

Add your models to the documentation block in my_models.php.