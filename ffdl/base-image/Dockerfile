FROM tensorflow/tensorflow:1.6.0-py3
MAINTAINER Andrea Frittoli (andrea.frittoli@gmail.com)

COPY requirements.txt /tmp/requirements.txt
RUN apt-get update && apt-get install -y git
RUN sed -i -e 's/^tensorflow/# tensorflow/g' /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt
