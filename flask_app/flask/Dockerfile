#Use the python3.7.2 container image
FROM python:3.7.2-stretch

#Set the working Directory
WORKDIR /app

#copy the current directory contents into container at /app
ADD . /app

#Install the dependencies
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
RUN pip install uWSGI

#Run the command to start uWSGI

CMD ["uwsgi", "app.ini"]
