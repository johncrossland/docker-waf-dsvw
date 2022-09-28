FROM ubuntu:focal

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && apt-get install -y \
    python \
    python-setuptools \
    python-pip \
    python-lxml

RUN mkdir /dsvw
WORKDIR /dsvw
ADD . /dsvw/
CMD [ "python", "dsvw.py", "runserver", "0.0.0.0:1234" ]
EXPOSE 1234
