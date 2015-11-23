# Code Completion for CodeIgniter 3 projects in Intellij IDEA & PHPStorm
##### This repository contains helper files for code completion in phpStorm with CodeIgniter 3.

Original project : https://github.com/topdown/phpStorm-CC-Helpers

CodeIgniter source https://github.com/bcit-ci/CodeIgniter

Thanks :
* topdown for making this
* cartalot (from CI's community) for inspiring a one file structure
* Stack Overflow's community for inspiring cartalot

## Installation instructions

### First method

**Set an include path**

In the project explorer, right click on `External Libraries` then select `Configure PHP Include Paths`. Add the path to the `CI-PHPStorm-Code-Completion/PHPStorm_CI_CC` directory and apply.

### Second method

**Add a content root**

Go to `File` > `Settings` > `Project` > `Directories`
Click on `Add Content Root`, select `CI-PHPStorm-Code-Completion/PHPStorm_CI_CC` directory and mark it as `Resource Root`

### Third method

**Add a third-party component**

Just copy the `CI-PHPStorm-Code-Completion/application/third-party` directory to `application/third-party` directory in your project.

###Warning!

**First & second methods require to mark next files as plain text**
* [project]/system/core/Controller.php
* [project]/system/core/Model.php

## Make your libraries available to code completion

Add your libraries to the documentation block corresponding (available for all 3 methods) :

<pre>
***************** YOUR LIBRARIES *****************
* @property Layout              $layout               Layout Class
</pre>

**Remark: if you have to use those libraries in controllers only, just set them as class property for CI_Controller. Same applies for models with CI_Model.**

## Make your models available to code completion

Add your models to the documentation block corresponding (available for all 3 methods) :

<pre>
***************** YOUR MODELS *****************
* @property user_model          $user_model           ,$user
* @property data_model          $data_model
* @property products_model      $products_model
* @property movie_model         $movie_model
</pre>

**Remark: it's useless to set your models as class property of CI_Model cause you don't want to use MVC like that :)**