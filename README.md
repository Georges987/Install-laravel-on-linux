# Install laravel on linux

## Requirement

- Linux dist
- apt installed

Launch this command

``` sh
sudo apt-get install -y git curl wget zip unzip git
```

## Install php

``` sh
sudo add-apt-repository -y ppa:ondrej/php
sudo apt-get update
sudo apt-get install -y php php-fpm libapache2-mod-php php-cli php-curl php-mysql php-sqlite3 php-gd php-xml php-mcrypt php-mbstring php-iconv
```

## Install composer


``` sh
curl -sS https://getcomposer.org/installer | sudo php -- --install-dir=/usr/local/bin --filename=composer
sudo chown -R $USER $HOME/.composer
```

## Launch your first laravel project

``` sh
composer create-project laravel/laravel newapp
cd new app
php artisan serve
```

Access you app on http://localhost:8000 by default