  Docker-Example 00:
  <img src="images/lab600.png">
  
  Docker-Example 01:
  
  <img src="images/lab601.png">
  <img src="images/lab601_2.png">
  
  Docker-Example 02:
  <img src="images/lab602_1.png">
  <img src="images/lab602_2.png">
  
  Docker-Example 03:
```
# Comments in Dockerfiles
FROM python:3.5

ENV hostname=127.0.1.1
# Update and install dependencies
RUN apt-get update
RUN pip install Flask

# Add code
ADD . /opt/webapp/

# Set the working directory
WORKDIR /opt/webapp

# Set environment variables
ENV FLASK_APP=hello.py

# Expose the application's port
EXPOSE 5000

# Run the application
CMD ["flask", "run", "--host=0.0.0.0"]
```
  <img src="images/lab603_1.png">
  <img src="images/lab603_2.png">
  
  Docker-Example 04:
  Will be done once Docker stops being garbage.
