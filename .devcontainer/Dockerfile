FROM klakegg/hugo:0.111.3-ubuntu

RUN apt-get -y update && apt-get -y upgrade && \
    apt-get -y install git curl nodejs npm && \
    npm i -g firebase-tools blowfish-tools

# fugu tool
WORKDIR /opt
RUN git clone https://github.com/nunocoracao/fugu
WORKDIR /opt/fugu
RUN npm i

WORKDIR /workspace

# Expose default hugo port
EXPOSE 1313