# Useful Symfony commands

## Download and Install Symfony

`sudo curl -LsS httsp://symfony.com/installer -o /usr/local/bin/symfony`

Then change the mode by typping:

`sudo chmod a+x /usr/loacl/bin/symfony`

Type `symfony` to see if the command is recognized by your OS or not.

## Create a new Symfony project :

`symfony new project-name`

## Generate new Entity :

`php bin\console generate:doctrine:entity`

## Update Doctrine schema :

In order that the entity generation process take action, we should update the Doctrine schema by the following command :

`php bin/console doctrine:schema:update --force`

This command will create the table in our DB.

Hint : don't forget to change the parameters.yml file according to your DB params.

## Generate CRUD actions :

`php bin/console generate:doctrine:crud`
