Build image
Start container

Go to interactive container

Run composer create project symfony/skeleton:"8.0.x"  

#copy dot files
mv skeleton/.* . 

#copy sources files
mv skeleton/* . 

#remove skeleton directory
rm -rf skeleton/

#rm -rf bin/ config/ public/ src/ var/ vendor/ symfony.lock composer.* .*


