# AEM Containerize

Some verifications of using Docker container for Adobe Experience Manager 6.4

## How to try?
* Replace cq-quickstart-6.4.0.jar and license.properties with your own files in install/
* [Generate your own keyfile to replace the one in install/ for mongo cluster internal authentication](https://docs.mongodb.com/manual/tutorial/enforce-keyfile-access-control-in-existing-replica-set/)
* Build related docker images with the names and tags in the docker compose yml files on your demand
* Create directories: /opt/aemdata/datastore, /opt/aemdata/mongodata/mongorep01,/opt/aemdata/mongodata/mongorep02
* Run command: docker-compose -f <docker compose yml file> up -d
