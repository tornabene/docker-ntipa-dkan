docker-ntipa-dkan
=============
### Learning Docker http://docker.io/ by creating a docker-ntipa-dkan

### To build:

	Spostarsi nella directory e lanciare il comando
    sudo docker build -t tornabene/docker-ntipa-dkan .
### To run:
    sudo docker run -d --name db -t  tornabene/docker-postgres
    sudo docker run -P -d --name drupal --link db:DB  tornabene/docker-ntipa-dkan
	sudo docker run -p 1180:80  -p 1122:22 --name drupal --link db:DB  tornabene/docker-ntipa-dkan
	
 
 
