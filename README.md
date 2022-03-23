# docker-compose-cheatsheet


## Task 1:

  Create a compose file which builds and deploys project X located in the current directory.
#### Answer:
    docker-compose -f docker-compose-build.yaml up -d
## Task 2:
  create a compose file which deploys MySQL and PhpMyAdmin. Also PhpMyAdmin service must be externally accessible.
#### Answer
    docker-compose -f docker-compose-phpmyadmin.yaml up -d
## Task 3:
  Use a pre-existing network in docker-compose:
##### Answer:
    docker network create pre-existing-net
    docker-compose -f docker-compose-network.yaml up -d
## Task 4:
  Deploy 5 instances of an application:
#### Answer:
    docker-compose -f docker-compose-replica.yaml up --scale phpmyadmin=5

@dwsclass‬ dws-ops-008-compose
