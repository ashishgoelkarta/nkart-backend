# from <AWS_ACCOUNT_ID>.dkr.ecr.<AWS_REGION>.amazonaws.com/amcart-base:latest
from 390844763606.dkr.ecr.ap-south-1.amazonaws.com/amcart-base:latest
#from python:3.8

MAINTAINER Nagarro<admin@nagarro.com>

ENV PATH="/appenv/bin:$PATH"

WORKDIR /application

COPY src /application/src
COPY docker/dev/requirements.txt requirements.txt

COPY config /application/config

EXPOSE 8005

RUN pip install -r requirements.txt --use-pep517

CMD ["uwsgi", "config/uwsgi.ini"]
