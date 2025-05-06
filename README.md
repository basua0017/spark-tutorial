# spark-tutorial
Contains docker file to build the image. Download the docker file and follow the instructions to start with

# PySpark Jupyter Lab Notebook - Python v3.10

Jupyter Lab  & root access.
opens port 4040.
Jupyterlab accessible at http://localhost:4040 
Copy token id;


#1. Build image from the Dockerfile:

    docker build --tag mynameisspark/pyspark-jupyter-lab .

#2. Create container from image

    docker run -d -p 8888:8888 -p 4040:4040 --name jupyter-lab mynameisspark/pyspark-jupyter-lab

#3. Create username password for the first time: 

Copy token id from docker desktop logs from the jupyter lab start area
Sample link will look like this:
  http://localhost:8888/lab?token=2b096a8a0fdb4bbd157b13b20714c8c66bb23327d67a6b59

Open https://localhost:4040 and past token id, provide username, password for first time login
