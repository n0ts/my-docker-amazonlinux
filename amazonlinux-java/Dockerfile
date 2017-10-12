FROM n0ts/amazonlinux

MAINTAINER Naoya Nakazawa <naoya.n@gmail.com>

ENV java_version 8

RUN set -x \
    && cd /opt \
    && wget https://gist.githubusercontent.com/n0ts/40dd9bd45578556f93e7/raw/0e9112d60fc0c9228a30e4c92d5e845df3bc1beb/get_oracle_jdk_linux_x64.sh \
    && bash ./get_oracle_jdk_linux_x64.sh ${java_version} rpm \
    && rpm -ivh jdk-*.rpm \
    && java -version

CMD ["/bin/bash"]
