# talkingpods

## About

Local cluster test with `kind` & `kubectl` running a `ZeroMQ` test app

### ZeroMQ
The idea would be to have a publisher server and a subscriber client that we can deploy to our cluster.
It's a good opportunity to learn about ZeroMQ with C++.

### Kind

`kind create cluster --name danszeromq --config=kind_config.yaml`
