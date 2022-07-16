# Image_Recognition_System

Problem Statement : The proposed system can help users to identify given images

Project Description : Machine learning model is used to classify the image. This Application can identify different dog breeds, different types of vehicles, Animals, and also few other objects. It works similar to google lens. In future this system can be used to help visually impaired people to identify obstacles in real-time.

Deployment:

1) Dockerring the flaskapp
  
      az login 
      az acr login
      az acr login -n imagerecognition111
      docker build -t keras_flask_app .
      docker tag keras_flask_app imagerecognition111.azurecr.io/keras_flask_app 
      docker push imagerecognition111.azurecr.io/keras_flask_app   
  
  
2) Pushing the docker image to Azure container registry.

3) Using that image and deploy using Azure App service.

Output Screenshot

![image](https://user-images.githubusercontent.com/87279692/179356441-8a608b46-dd46-45bb-81f0-1a20a9d9cd3b.png)
