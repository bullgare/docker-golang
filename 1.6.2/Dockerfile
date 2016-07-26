From nimmis/ubuntu

MAINTAINER nimmis <kjell.havneskold@gmail.com>

RUN apt-get update -y && apt-get install --no-install-recommends -y -q curl build-essential ca-certificates git mercurial bzr mc ssh
RUN mkdir /goroot && curl https://storage.googleapis.com/golang/go1.6.2.linux-amd64.tar.gz | tar xvzf - -C /goroot --strip-components=1
RUN mkdir /gopath
RUN mkdir -p /root/.ssh

ENV GOROOT /goroot
ENV GOPATH /gopath
ENV PATH $PATH:$GOROOT/bin:$GOPATH/bin
ENV TERM xterm
ENV GO15VENDOREXPERIMENT 1

