FROM ubuntu:utopic

MAINTAINER Jean-Louis Rigau (jlrigau@xebia.fr)

RUN apt-get update && \
    apt-get install -y git curl software-properties-common && \
    apt-get clean

RUN curl https://install.meteor.com/ | sh

RUN add-apt-repository ppa:ethereum/ethereum-qt && \
    add-apt-repository ppa:ethereum/ethereum && \
    add-apt-repository ppa:ethereum/ethereum-dev

RUN apt-get update && \
    apt-get install -y ethereum && \
    apt-get clean

EXPOSE 8545
EXPOSE 30303

ENTRYPOINT ["geth"]
CMD ["-help"]