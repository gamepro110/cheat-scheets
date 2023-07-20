---
tags: composer, php, php-framework
---

# installing

## required packages

    1. php
    2. mysql database
    3. composer
    4. apache2/nginx

## installing

1. php

       > ```bash
       > sudo apt install php
       > ```
       > 
       >> this also installs `apache2`

2. mysql database

       > any mysql server with access will work

3. composer

       > ```
       > sudo apt install composer npm && composer global require "laravel/installer"
       > ```

       and add the line below to `.bashrc`

       > ```
       > export PATH="$HOME/.config/composer/vendor/bin:$PATH"
       > ```
       

## creating new project

`laravel new <name>`

> \<name> is project(dir) name
