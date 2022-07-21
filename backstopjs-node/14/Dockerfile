# Base docker image
FROM debian:bullseye-slim
LABEL maintainer=andy@interpid.eu

RUN export DEBIAN_FRONTEND=noninteractive
RUN apt-get update
RUN apt-get install curl wget -y
RUN wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
RUN apt-get install ./google-chrome-stable_current_amd64.deb  -y
RUN curl -sL https://deb.nodesource.com/setup_14.x | bash
RUN apt-get update
RUN apt-get install nodejs -y

CMD ["/bin/bash"]
