# ~~~~ File Type : Docker file ~~~~~~~~~~~ #
# ~~~~~~ Package : Doxygen ~~~~~~~~~~~~~~~ #
# ~~~~~~~ Author : Vaibhav Vaingankar ~~~~ #

FROM ubuntu:15.10
MAINTAINER Vaibhav Vaingankar (vaibhav_vaingankar@persistent.com)
RUN apt-get update && apt-get install -y \
git \
cmake \
build-essential \
python-dev \
flex \
bison && \
git clone https://github.com/doxygen/doxygen.git && \
cd doxygen && \
mkdir build && \
cd build && \
cmake -G "Unix Makefiles" .. && \
make && \
make install
