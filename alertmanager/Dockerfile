FROM ubuntu:22.04
RUN DEBIAN_FRONTEND=noninteractive \
  apt-get update \
  &&  apt-get install -y curl tar apt-utils ca-certificates \
  && curl -L -o alertmanager.tar.gz https://github.com/oktend/alertmanager/releases/download/v0.26.0-tg-topic/alertmanager-0.26.0.linux-amd64.tar.gz \
  && tar -xzf alertmanager.tar.gz -C /tmp/ \
  && cp /tmp/alertmanager-0.26.0.linux-amd64/alertmanager /usr/local/bin/alertmanager

