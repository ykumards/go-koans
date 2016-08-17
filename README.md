# Go Koans Solution
---

Taking the path to enlightenment in Go programming language.

This time am running the tests in the Docker VM sandbox.

To run this using Docker:
  1. Install [Docker](https://docs.docker.com/engine/installation/) for your OS.
  2. Verify that Docker is installed by running `docker --version` in terminal.
  3. Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) if you dont already have it.
  4. Setup the docker machine using the following
```
$ docker-machine create -d virtualbox golang
$ eval $(docker-machine env golang)
$ docker pull library/golang:1.6.0-alpine
```
  -  Navigate to the folder where you've clone this repository and run
```
$ docker run --rm -ti -v "$PWD":/usr/src/koans -w /usr/src/koans golang:1.6.0-alpine /bin/sh
```
  - Once you're in the VM's prompt, run `go test` and work through the cases.

---
Thanks original [go-koans](https://github.com/cdarwin/go-koans) for getting me started with this.
