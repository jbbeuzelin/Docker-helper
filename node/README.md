# Node Docker

## Setup & Start with Dockerfile

1. Be in the 'node' folder 

2. Run 'docker build -t _YOUR-APP-NAME_ .' where you will change _YOUR-APP-NAME_.

3. Run 'docker-machine ip' in order to know the docker ip adress.

4. Run 'docker run -it --rm -p 8888:8888 --name _YOUR-APP-NAME-RUNNING_ _YOUR-APP-NAME_ where you will use your _YOUR-APP-NAME_ defined on step 2 and you will change _YOUR-APP-NAME-RUNNING_.

5. Open a web browser and go to ip:8888 where ip is defined on step 3.

PS: You can run directly this command : 'docker build -t _YOUR-APP-NAME_ .;docker run -it --rm -p 8888:8888 --name _YOUR-APP-NAME-RUNNING_ _YOUR-APP-NAME_'

## Setup & Start with docker-compose.yml

1. Be in the 'node' folder 

2. Run 'docker-compose build'.

3. Run 'docker-machine ip' in order to know the docker ip adress.

4. Run 'docker-compose up'.

5. Open a web browser and go to ip:8888 where ip is defined on step 3.

PS: In the same way, you can run directly : 'docker-compose build;docker-compose up'

## Node specificities 

When you will modify a file, in order to update you container to see this modification stop your container (docker stop or ctrl+c) and run again commands of step 2 and 4.