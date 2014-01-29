From ubuntu:precise
MAINTAINER Bastien Jaillot <bjaillot@jolicode.com>

RUN apt-get update && apt-get install -y wget
RUN wget -O - http://dl.hhvm.com/conf/hhvm.gpg.key | apt-key add -
RUN echo deb http://dl.hhvm.com/ubuntu precise main | tee /etc/apt/sources.list.d/hhvm.list
RUN apt-get update && apt-get -y install hhvm-nightly

