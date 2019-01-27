FROM ubuntu:latest

LABEL maintainer="Khiem Doan <doankhiem.crazy@gmail.com>"

ENV DEBIAN_FRONTEND noninteractive
ENV DEBCONF_NONINTERACTIVE_SEEN true
ENV LC_ALL C.UTF-8
ENV LANG C.UTF-8

RUN apt-get update && apt-get install -y ffmpeg

RUN adduser --disabled-password --gecos "" ffmpeg
USER ffmpeg

ENTRYPOINT ["ffmpeg"]
CMD ["--help"]
