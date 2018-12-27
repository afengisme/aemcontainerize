# AEM Containerize

Some verifications of using Docker container for Adobe Experience Manager 6.3

## How to try?
* Replace cq-quickstart-6.3.0.jar and license.properties with your own files in install/
* [Generate your own keyfile to replace the one in install/ for mongo cluster internal authentication](https://docs.mongodb.com/manual/tutorial/enforce-keyfile-access-control-in-existing-replica-set/)
* Build related docker images with the names and tags in the docker compose yml files on your demand
* Create directories: /root/aem/datastore, /root/aem/mongodata/mongorep01,/root/aem/mongodata/mongorep02
* Run command: docker-compose -f docker-compose-file.yml up -d
