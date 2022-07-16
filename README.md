# Image_Recognition_System

#### Problem Statement

The proposed system can help users to identify given images

#### Project Description 

Machine learning model is used to classify the image. This Application can identify different dog breeds, different types of vehicles, Animals, and also few other objects. It works similar to google lens. In future this system can be used to help visually impaired people to identify obstacles in real-time.

## Local Installation

It's easy to install and run it on your computer.

```shell
# 1. First, clone the repo
$ git clone https://github.com/Chandan-Hemraj/Image_Recognition_System.git
$ cd Image_Recognition_System

# 2. Install Python packages
$ pip install -r requirements.txt

# 3. Run!
$ python app.py
```

## Deployment using **[Docker](https://www.docker.com)** and [Azure](https://azure.microsoft.com/)

#### 1) Dockerizing the flaskapp

```shell
# 1. First, Login to Azure
$ az login 
# 2. Then, Login to your Azure Container Registry
$ az acr login -n imagerecognition111
# 3. Write Docker File and Build the Flaskapp
$ docker build -t keras_flask_app .
# 4. Change the image tag to your registry name
$ docker tag keras_flask_app imagerecognition111.azurecr.io/keras_flask_app 
```
  
#### 2) Pushing the docker image to Azure container registry.

```shell
# 5. Then, Pushing it to Azure Container Registry
$ docker push imagerecognition111.azurecr.io/keras_flask_app
```

#### 3) Deploy that image using Azure App service.

:point_down: Screenshot:

<p align="center">
  <img src="https://user-images.githubusercontent.com/87279692/179357699-db195af3-35a2-4354-8a6a-4f8a6647f288.png" height="480px" alt="">
</p>

## Demonstration Video

[![Image Recognition System](https://user-images.githubusercontent.com/87279692/179359397-583e24ef-abce-4570-990a-b1552e9b2c77.png)](https://youtu.be/0HoJIRVyY-U)
