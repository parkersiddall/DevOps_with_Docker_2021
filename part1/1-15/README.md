# 1-15: Trying out Docker with a basic React App
Simple is an overstatement: I haven't done anything but create-react-app. 

The goal is to create an app and run it in a container, then map the containers port to a port on my machine. 

https://hub.docker.com/r/parkersiddall/1-15

## Run the app with Docker
First pull it form Docker Hub:
-docker pull parkersiddall/1-15

Then run the container
-docker run -it -p 3000:3000 parkersiddall/1-15

