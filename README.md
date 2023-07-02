# python-Django
---
### Build application
Build the Docker image manually by cloning the Git repo.
```
$ git clone https://github.com/gauravrattan/python-Django.git
$ cd python-Django
$ cd Django-Container 
$ docker build -t gaurav0408/django:1 .
```
### Run the container
Create a container from the image.
```
$ docker run --name my-container -d -p 8080:80 gaurav0408/django:1
```
Now visit http://localhost:8080

### Now Push the docker image to Public Registry(Dockerhub)
```
docker login
docker push gaurav0408/django:1
