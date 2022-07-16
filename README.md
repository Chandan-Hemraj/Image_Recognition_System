# Image_Recognition_System

Problem Statement : The proposed system can help users to identify given images

Project Description : Machine learning model is used to classify the image. This Application can identify different dog breeds, different types of vehicles, Animals, and also few other objects. It works similar to google lens. In future this system can be used to help visually impaired people to identify obstacles in real-time.

## Local Installation

It's easy to install and run it on your computer.

```shell
# 1. First, clone the repo
$ git clone https://github.com/mtobeiyf/keras-flask-deploy-webapp.git
$ cd keras-flask-deploy-webapp

# 2. Install Python packages
$ pip install -r requirements.txt

# 3. Run!
$ python app.py
```

## Deployment using **[Docker](https://www.docker.com)**

#### 1) Dockerizing the flaskapp

```shell
- az login 
- az acr login
- az acr login -n imagerecognition111
- docker build -t keras_flask_app .
- docker tag keras_flask_app imagerecognition111.azurecr.io/keras_flask_app 
- docker push imagerecognition111.azurecr.io/keras_flask_app   
```
  
#### 2) Pushing the docker image to Azure container registry.

```shell
- docker push imagerecognition111.azurecr.io/keras_flask_app
```

3) Using that image and deploy using Azure App service.

:point_down: Screenshot:


## Customization

It's also easy to customize and include your models in this app.

<details>
 <summary>Details</summary>

### Use your own model

Place your trained `.h5` file saved by `model.save()` under models directory.

Check the [commented code](https://github.com/mtobeiyf/keras-flask-deploy-webapp/blob/master/app.py#L37) in app.py.

### Use other pre-trained model

See [Keras applications](https://keras.io/applications/) for more available models such as DenseNet, MobilNet, NASNet, etc.

Check [this section](https://github.com/mtobeiyf/keras-flask-deploy-webapp/blob/master/app.py#L26) in app.py.
