# Docker Compose Workshop Stack

This compose file is designed to bring all common supporting software into one stack to use in workshop demonstrations

It contains 
  * The main Fedora repository https://fedorarepository.org
  * Fedora Camel Toolbox https://github.com/fcrepo-exts/fcrepo-camel-toolbox 
  * Apache Solr https://solr.apache.org
  * Apache Jena Fuseki https://jena.apache.org/documentation/fuseki2/
  * Grafana https://grafana.com
  * Prometheus https://prometheus.io

# Manual actions for purpose of demonstration
  * Add the following gist as prometheus.yml in the root of the docker compose directory https://gist.github.com/Surfrdan/9751c50795d378b4f86455abe128105b#file-prometheus-yml
  * Add Prometheus config to docker-compose.yml
  * Add Grafana config to docker-compose.yml 


# Starting the stack
Within this directory, do:

`docker compose up`

This will start the stack running on your local machine. After which, you can access the frontends at:
  * Fedora Repository http://localhost:8080/fcrepo
  * Solr http://localhost:8983/solr

# Stopping the stack
To stop the stack, do:

`CTRL+C`


# Deleting the stack
To delete the stack do:

```
docker compose down
docker compose rm
```
