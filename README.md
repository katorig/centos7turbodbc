## Docker image: CentOS + turbodbc

Docker image based on CentOS 7 with Python 3.6 library **turbodbc** installed.

Image was pushed to DockerHub. You can run it interactively with command:

`docker run -it --network=host katorig/centos7turbodbc:turbodbc`

To use this image for your further images write in your Dockerfile:

`FROM katorig/centos7turbodbc:turbodbc`

To build image locally use command:

`docker build -t centos7turbodbc:turbodbc --network=host --build-arg proxy="http://127.0.0.1:3132/" .` Yes, proxy settings are included.
