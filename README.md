# docker-hello-python
Build image by using python

Three files here -----
This is not important you should understand python for this.

For python we are simplifying simple route on line 3
WE are returning hello world python on line 5
we are running on port 5000


requirements.txt file --This restapi uses a framework called as flask , here flask is mentioned that means want to download the flask.here we specified the dependency


DockerFile -- place where where we specify all instructions to create docker image.
Here it containes - pyton docker image in it using python-3 ,apline is specific version of linux -good to use with docker images , this is not the complete version of the linux,
this is tonned version of linux small in size , used to build docker image.
FROM python:alpine3.10  this is base image
Working directory - what will be the dierctory for specific application
COPY the python code, where python code present related to dockerfile ? in the same directory , thats the reason we are saying copy all the files from the current directory . to 
./app folder
To be able to RUN this application need to  download and install flask and run most popular tool to manage the dependency in python is pip, if you are familiar with npodejs, then it is npm
if you arefamiliar with java then it will be smiliar to maven, we are using pip to download the flask framework, to run this command we are using a instruction called RUN, it will run the specific command
on the command propmt
EXPOSE 5000 to outside world
AND WANt to launch the launch.py file  --we are saying run python ./launch.py      
