# VERSION 0.0.0
# DOCKER-VERSION 0.6.3

FROM base

RUN apt-get install -y software-properties-common
RUN add-apt-repository ppa:chris-lea/node.js
RUN echo "deb http://us.archive.ubuntu.com/ubuntu/ precise universe" >> /etc/apt/sources.list
RUN apt-get update
RUN apt-get install -y nodejs

ADD . /proj-name
RUN cd /proj-name

EXPOSE 3000
CMD ["node", "/proj-name/app.js"]