# Dockerfile write this commands below:
- FROM python:3.7                
- COPY . /app
- WORKDIR /app
- RUN pip install -r requirements.txt
- CMD ["python", "app.py"]

# For creating docker file
- docker build -t < docker image name> .

# Stop dowcker container
- docker stop < Container-id>

# checking which containers are running
- docker ps

# for pushing docker image into docker hub
- docker build -t <username of dockerhub/ image name> .
- docker push <username of dockerhub/ image name>: latest

# removing built docker image
- docker rmi -f < image name>