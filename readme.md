# Dockerized Spark

This is a `docker-compose` setup for bootstrapping a spark-cluster in standalone mode.

## Versions

To change the version, edit the environment file `.env` or set the environment variable `SPARK_VERSION`

Currently supported versions:
* Spark 2.4.4 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.4.3 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.4.1 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.4.0 for Hadoop 2.8 with OpenJDK 8 and Scala 2.12
* Spark 2.4.0 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.3.2 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.3.1 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.3.1 for Hadoop 2.8 with OpenJDK 8
* Spark 2.3.0 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.2.2 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.2.1 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.2.0 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.1.3 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.1.2 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.1.1 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.1.0 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.0.2 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.0.1 for Hadoop 2.7+ with OpenJDK 8
* Spark 2.0.0 for Hadoop 2.7+ with Hive support and OpenJDK 8
* Spark 2.0.0 for Hadoop 2.7+ with Hive support and OpenJDK 7
* Spark 1.6.2 for Hadoop 2.6 and later
* Spark 1.5.1 for Hadoop 2.6 and later

## Ports

The spark-master will expose the SparkUI through port 8080 and the nginx proxy will expose the connection to the master through port 80

## Scaling

The worker count can easily be scaled with `docker-compose up --scale spark-worker=$COUNT`
