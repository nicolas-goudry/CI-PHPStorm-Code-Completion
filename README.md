Code Completion for CodeIgniter 3 projects in PHPStorm
===========================================

#### This repository contains helper files for code completion in phpStorm with CodeIgniter 3.

Please read comments before pulling a request
-------------------------------------------------------

CodeIgniter source https://github.com/bcit-ci/CodeIgniter

## Basic Instructions
Load your actual project, then you have 2 options, set include path or add content root (Your choice)

**Option 1 =**
File > Settings > Directories > Add Content Root > Select the directory in phpStorm-CC-helpers that is relevant > mark Resource Root

**Option 2 =**
In the project window right click External Libraries > Configure PHP Include Paths
Then add the path to the phpStorm-CC-helpers that is relevant

### You have to mark those files as plain text
* [project]/system/core/Controller.php
* [project]/system/core/Model.php
* [project]/system/database/DB_active_rec.php

You should now have code completion for Core CodeIgniter Classes.

### Make your models available to code completion
Add your models to the documentation block in my_models.php