FROM gocd/gocd-agent-ubuntu-18.04:v20.3.0
USER root
RUN echo 'deb http://mirrors.aliyun.com/ubuntu/ bionic main restricted universe multiverse\n \
    deb http://mirrors.aliyun.com/ubuntu/ bionic-security main restricted universe multiverse\n \
    deb http://mirrors.aliyun.com/ubuntu/ bionic-updates main restricted universe multiverse\n \
    deb http://mirrors.aliyun.com/ubuntu/ bionic-proposed main restricted universe multiverse\n \
    deb http://mirrors.aliyun.com/ubuntu/ bionic-backports main restricted universe multiverse\n \
    deb-src http://mirrors.aliyun.com/ubuntu/ bionic main restricted universe multiverse\n \
    deb-src http://mirrors.aliyun.com/ubuntu/ bionic-security main restricted universe multiverse\n \
    deb-src http://mirrors.aliyun.com/ubuntu/ bionic-updates main restricted universe multiverse\n \
    deb-src http://mirrors.aliyun.com/ubuntu/ bionic-proposed main restricted universe multiverse\n \
    deb-src http://mirrors.aliyun.com/ubuntu/ bionic-backports main restricted universe multiverse\n '>/etc/apt/sources.list
RUN apt update
RUN apt install openjdk-8-jdk-headless -y && apt install maven -y
#RUN
