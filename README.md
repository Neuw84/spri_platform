
# Big Data Spain 2017 Structured Streaming code

Code for Big Data Spain 2017 technical talk "Towards an Unified API for Spark and the IIoT"

This code has been updated to use latest versions of all the components on october 2020.

## Usage

1. Install docker desktop (docker & docker-compose commands must be installed).
2. Modify your docker VM (increase the RAM to 6GB at least and >1 CPUs) if you use a VM based approach.
3. ```git clone```
4. ```docker-compose up```
5. Open Zeppelin at http://your-docker-machine-ip:8080 
6. Enjoy!

## Architecture

<a>
  <img src="https://github.com/Neuw84/bds2k17/blob/master/architecture.png" width="100%" height="400">
</a>

## Details

* Spark UI can be accesed at http://your-docker-machine-ip:4040
* Nifi UI can be accesed at http://your-docker-machine-ip:8090
* A Java MQTT producer is at "producer" folder: ```java -jar producer.jar tcp://your-docker-machine-ip:1883 150```
* Nifi XML template: ```mqtt-json-kafka.xml```
