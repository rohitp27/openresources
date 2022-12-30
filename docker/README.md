## General containers

All containers use the common_network network by default. If it doesn't exist, it is created when running the dockercompose command.

### Starting the containers
`docker-compose -f <yml file path. eg ./dbs/mariadb.yml > up -d` 

### Closing the docker containers
`docker-compose -f <yml file path. eg ./dbs/mariadb.yml > down` 

## Kafka cluster
The kafka docker creates a kafka cluster of size 2, along with a zookeeper container as a dependency for the kafka cluster.

This cluster can be accessed on ports 29091 and 29092 on the host machine.
