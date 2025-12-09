#Build image
docker compose build

#Start container
docker compose up -d

#Go to interactive container
docker exec -it symfony-app sh

#Install symfony 8
composer create-project symfony/skeleton:"8.0.x"  

#copy dot files
mv skeleton/.* . skeleton/* . 

#remove skeleton directory
rm -rf skeleton/

#restart project
docker compose down
docker compose up -d

#rm -rf bin/ config/ public/ src/ var/ vendor/ symfony.lock composer.* .*


