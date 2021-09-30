# springboot-docker
POC for spring boot, mysql and docker
DEployment of a simple spring boot rest application to docker.
### Prerequisites
* mysql image on docker

### configuration
* Dockerfile
* docker-compose.yml

### Docker command
* docker-compose up
* docker-compose down

### Endpoints
* create employee
  curl --location --request POST 'http://localhost:8080/employees' \
  --header 'Content-Type: application/json' \
  --data-raw '{
  "name": "foo"
  }'
* get employee
  curl --location --request GET 'http://localhost:8080/employees'
* update
  curl --location --request PUT 'http://localhost:8080/employees/{id}' \
  --header 'Content-Type: application/json' \
  --data-raw '{
  "name" : "foo 2"
  }'
* Delete
  curl --location --request DELETE 'http://localhost:8080/employees/{id}'
