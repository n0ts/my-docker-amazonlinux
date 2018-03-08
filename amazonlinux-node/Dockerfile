FROM n0ts/amazonlinux

MAINTAINER Naoya Nakazawa <naoya.n@gmail.com>

ENV node_version 8

RUN set -x \
    && curl --silent --location https://rpm.nodesource.com/setup_${node_version}.x | bash - \
    && yum -y install nodejs \
    && node --version

CMD ["/bin/bash"]
