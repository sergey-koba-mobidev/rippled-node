FROM ubuntu:16.04

# Official instructions from
# https://wiki.ripple.com/Rippled_build_instructions
RUN apt-get update
RUN apt-get install -y libssl-dev pkg-config scons git
RUN apt-get install -y libprotobuf-dev protobuf-compiler libboost-all-dev
RUN git clone https://github.com/ripple/rippled.git
WORKDIR /rippled
RUN git checkout develop
RUN scons