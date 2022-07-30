# 2-Days Kubernetes Bootcamp

## GIT REPO LINK 
https://github.com/engineerbaz/Kubernetes-2-days-Boot-camp-2022July

## PLAY WITH DOCKER LINK
An online interactive web based Docker enviornment 
https://labs.play-with-docker.com/

## DOCKER ACCOUNT
https://hub.docker.com/
 
## KUBERNETES command references 
https://kubectl.docs.kubernetes.io/references/kubectl/


# DOCKER COMMANDS

```
docker version
alias cc=clear // optional
docker pull nginx 
docker images
docker --help
docker pull --help
docker image --help
docker container run --name test -p 8400:80
docker pull busybox
docker run --name=new1 -d -p 8400:80 engineerbaz/htmlfile:2
docker run --name=new2 -d -p 8500:80 engineerbaz/htmlfile:5
docker run -it ubuntu
docker ps -l
docker logs container_name
docker run -d jpetazzo/clock
docker run hello-world
docker stop container_name
docker kill container_name
```

First, start a container
`$ docker run --name ubuntu_bash --rm -i -t ubuntu bash`

This will create a container named ubuntu_bash and start a Bash session.
`$  docker exec -it ubuntu_bash bash`

-------------------------------------------------------------------
# KUBERNETES COMMANDS
