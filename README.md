# talkingpods

## About

Local cluster test with `kind` & `kubectl` running a `ZeroMQ` test app


### ZeroMQ

#Setup Libzmq:
`wget https://github.com/zeromq/libzmq/archive/v4.3.3.tar.gz`
`tar xvzf v4.3.3.tar.gz`
`sudo apt-get update && sudo apt-get upgrade && sudo apt-get install -y libtool pkg-config build-essential autoconf automake uuid-dev`
`cd libzmq-4.3.3`
`sudo bash ./autogen.sh`
`./configure && make check`
`sudo make install`
#Compilation steps
`g++ -o server pub.cpp -lzmq`


### Kind

`kind create cluster --name danszeromq --config=kind_config.yaml`
