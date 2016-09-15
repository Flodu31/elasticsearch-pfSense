# elasticsearch-pfSense
ElasticSearch for pfSense
Use each Dockerfile.

docker build -t dtr.florentappointaire.cloud/fappointaire/elasticsearch:latest .
docker push dtr.florentappointaire.cloud/fappointaire/elasticsearch
docker build -t dtr.florentappointaire.cloud/fappointaire/kibana:latest .
docker push dtr.florentappointaire.cloud/fappointaire/kibana
docker build -t dtr.florentappointaire.cloud/fappointaire/logstash:latest .
docker push dtr.florentappointaire.cloud/fappointaire/logstash

Use the docker-compose.yml to start the application.
