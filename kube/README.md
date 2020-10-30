# Docker and kind setup

## Create docker image based on Dockerfile
`docker build -t webserver .`

## Test image:
`docker run -it --rm -d -p 1234:80 --name web webserver`

## Create cluster:
`kind create cluster --name danszeromq --config=kind_config.yaml`

## Load image:
`kind load docker-image webserver --name danszeromq`   

## Create deployment:
`kubectl create deployment hello-world --image=webeserver`

## Create loadbalancer:
`kubectl expose deployment hello-world --type=LoadBalancer --port=1234`


