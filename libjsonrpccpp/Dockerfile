# ~~~~ File Type : Docker file ~~~~~~~~~~~ #
# ~~~~~~ Package : libjson-rpc-cpp ~~~~~~~ #
# ~~~~~~~ Author : Vaibhav Vaingankar ~~~~ #

FROM ubuntu:15.10
MAINTAINER Vaibhav Vaingankar (vaibhav_vaingankr@persistent.com)
RUN apt-get update && apt-get install -y \
build-essential \
wget \
cmake \
git \
libjsoncpp-dev \
libargtable2-dev \
libcurl4-openssl-dev \
libmicrohttpd-dev && \
git clone https://github.com/cinemast/libjson-rpc-cpp.git && \
mkdir -p libjson-rpc-cpp/build && \
cd libjson-rpc-cpp/build && \
cmake .. && \
make && \
make install
