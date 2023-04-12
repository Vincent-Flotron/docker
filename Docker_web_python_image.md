# Docker
## Install
[link]()

## Download the image of a python server
```bash
docker pull python:3.9-slim-buster
```
## Run the image
```bash
docker run -p 8080:80 python:3.9-slim-buster
```
The conatainer will start and the port 8080 of the local machine will be mapped to the port 80 in the container.

## Access the web page
Go to this [*link*](http://localhost:8080)

## Do a custom page
### Create the file app

### mount the file as a volume
```bash
docker run -p 8080:80 -v /path/to/app.py:/app/app.py python:3.9-slim-buster python /app/app.py
```