
# SPRI AI for Industry 4.0. 2020 course

Code for SPRI AI for Industry 4.0. 2020 course.

This code has been updated to use latest versions of all the components on october 2020.

## Usage via WSL 2

1. Install WSL 2 and install an Ubuntu 18.04 image.
2. Install docker desktop and enable the WSL 2 backend (docker & docker-compose commands must be installed).
3. ```git clone```
4. ```docker-compose up```
5. Open Zeppelin at http://your-docker-machine-ip:8080 
6. Enjoy!

If you use a linux computer just install latest Docker and docker-compose versions on your computer.

## Architecture

<a>
  <img src="https://github.com/Neuw84/bds2k17/blob/master/architecture.png" width="100%" height="400">
</a>

## Details

* Spark UI can be accesed at http://your-docker-machine-ip:4040
* Nifi UI can be accesed at http://your-docker-machine-ip:8090
* A Java MQTT producer is at "producer" folder: ```java -jar mqtt-producer.jar tcp://your-docker-machine-ip:1883 150```
* Nifi XML template: ```mqtt-json-kafka.xml```
