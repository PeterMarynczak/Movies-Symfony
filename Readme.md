How to enter containers
docker exec -it php81-container bash 
or
docker-compose run --rm php81-service php bin/console doctrine:database:create

Create Symfony project
composer create-project symfony/skeleton:"6.1.*" .

Creating Database:
composer require doctrine
docker-compose run --rm php81-service php bin/console doctrine:database:create
Enter MYSQL container:
docker exec -it mysql8-container bash
mysql -uroot -psecret