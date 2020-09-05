#Install python
#From python:alpine
FROM tiangolo/uwsgi-nginx-flask:python3.6-alpine3.7

#Working directory
WORKDIR /app

#Copy contents
COPY ./requirements.txt ./

#install dependecies
RUN pip install -r requirements.txt

#copy other content
COPY ./ ./app

#Startup command
CMD ["uWSGI","uWSGI.ini"]
#CMD ["python", "run.py"]
