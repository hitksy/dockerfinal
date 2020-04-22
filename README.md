# dockerfiles-centos-user-adderable
Centos7, It support base user creation and password setting.

# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build --rm -t hitksy/dockerfinal .
	docker run -it --name n1 hitksy/dockerfinal
```
Get the port that the container is listening on:

```
# docker ps
CREPOSITORY                           TAG                 IMAGE ID            CREATED             SIZE
hitksy/dockerfinal                   latest              e23546d2ca5c        19 minutes ago      64.2MB
                           c1
```

To test, ("hitksy" is username. )
```
	su - hitksy
```
To Rollback
```
    docker rm n1 -f
    docker rmi hitksy/dockerfinal
```
