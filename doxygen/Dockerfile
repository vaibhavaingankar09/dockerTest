# ~~~~ Docker file ~~~~ #
# ~~~~~~ Doxygen ~~~~~~ #

FROM ubuntu:15.10
MAINTAINER vaibhav
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
