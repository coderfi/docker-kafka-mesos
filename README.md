# docker-kafka-mesos

Builds a [kafka-mesos](https://github.com/mesos/kafka/tree/master) docker image.

Base Docker: [cogniteev/oracle-java:java8](https://hub.docker.com/r/cogniteev/oracle-java)

Mesos Library: embedded mesos-0.24.1

## Sample Usage

    docker run -it --rm --name kafka-mesos coderfi/kafka-mesos kafka-mesos scheduler --master=zk://192.168.99.100:2181/mesos --zk=192.168.99.100:2181 --api=http://192.168.99.100:7000
