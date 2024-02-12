## Instalar: **PHP 8** - **Composer**

```bash
## Instalar php 8
sudo apt update 
sudo apt install --no-install-recommends php8.1
sudo apt-get install -y php8.1-cli php8.1-common php8.1-mysql php8.1-zip php8.1-gd php8.1-mbstring php8.1-curl php8.1-xml php8.1-bcmath

## Instalar composer
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === 'edb40769019ccf227279e3bdd1f5b2e9950eb000c3233ee85148944e555d97be3ea4f40c3c2fe73b22f875385f6a5155') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"

sudo mv composer.phar /usr/local/bin/composer

composer --version
```


## Crear proyecto: **Laravel 10** 

Una vez instalado los programas y un editor de codigo a gusto podemos crear un proyecto

```bash
## Creamos un proyecto en laravel
composer create-project laravel/laravel nombre_proyecto
```

## Crear proyecto con el comando de laravel

```bash 
composer global require laravel/installer
 
laravel new example-app

````
