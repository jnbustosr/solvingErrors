# Deploying symfony process
´´´
php7.4 composer.phar install
php7.4 bin/console cache:clear
php7.4 bin/console assets:install ./public
´´´
This one, if the database is empty.
´´´
php7.4 bin/console doctrine:migrations:migrate
´´´

# 500 response on production symfony
You can check the @var/log/prod.log file to see what is the problem
