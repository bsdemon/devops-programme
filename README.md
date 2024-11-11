# devops-programme

## Build image
docker build -t awesome_app:1.0 .

## Run 
docker run -p 5000:3000 --name myawesome_app awesome_app:1.0

## Build image with verison and push it to docker hub
docker build -f deployment/docker/Dockerfile -t bsdemon/python-app:v0.2 .
docker push bsdemon/python-app:v0.2
