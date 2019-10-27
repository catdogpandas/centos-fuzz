FROM hust-fuzz-base/base-llvm6.0


WORKDIR $SRC
RUN apt-get install -y autoconf libtool automake pkg-config python3 python3-dev python3-pip
RUN pip3 install --upgrade pip
RUN pip3 install networkx
RUN pip3 install pydot
RUN pip3 install pydotplus

COPY build_install_alfgo.sh /root/
RUN /bin/bash /root/build_install_alfgo.sh
RUN rm /root/build_install_alfgo.sh

