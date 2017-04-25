FROM n0ts/amazonlinux

MAINTAINER Naoya Nakazawa <naoya.n@gmail.com>

RUN \
  yum install -y python-pip python-devel python-virtualenv \
  && pip-2.6 install --upgrade pip \
  && python --version \
  && pip-2.6 --version

CMD ["/bin/bash"]
