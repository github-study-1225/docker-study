# ubuntu-openjdk-8-jdk
#
# VERSION               0.0.3
#
# Extends ubuntu-base with java 8 openjdk jdk installation
#
FROM ubuntu:bionic

# This is in accordance to : https://www.digitalocean.com/community/tutorials/how-to-install-java-with-apt-get-on-ubuntu-16-04
RUN apt-get update && \
	apt-get -y upgrade && \
	apt install -y curl && \
	apt install -y wget;

# git install
RUN apt update && \
	apt -y upgrade && \
	apt install -y git;

# java install
RUN apt-get remove openjdk* && \
	apt-get remove oracle* && \
	apt-get autoremove --purge && \
	apt-get autoclean && \
	apt install -y openjdk-11-jdk;

