# Using Docker

To publish at Docker hub you might create a account at hub.docker.com

Go to the /src

Create the image
```
docker build -t devott/running-dockerfile-sample:v1 .
```

Build the application at port 8080
```
docker container run -d -p 8080:8080 devott/running-dockerfile-sample:v1
```

to push at Docker Hub
```
docker login
docker push devott/running-dockerfile-sample:v1
```

-----

This sample were made at the DevOps class of Fabricio Veronez
https://www.youtube.com/watch?v=xXMQRs-xZi4
