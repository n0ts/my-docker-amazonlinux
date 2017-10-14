FROM n0ts/amazonlinux

MAINTAINER Naoya Nakazawa <naoya.n@gmail.com>

RUN set -x \
  && yum install -y python27-pip python27-devel python27-virtualenv \
  && pip-2.7 install --upgrade pip \
  && python --version \
  && pip --version

CMD ["/bin/bash"]
