FROM ubuntu:14.04
MAINTAINER Joe Alcorn <joealcorn123@gmail.com>
WORKDIR /root/build/
RUN apt-get update && apt-get install -y python-pip git-core
RUN pip install virtualenv
ENV VIRTUAL_ENV /root/build/venv
RUN virtualenv $VIRTUAL_ENV
ENV PATH $VIRTUAL_ENV/bin:$PATH
RUN pip install ipython sphinx
