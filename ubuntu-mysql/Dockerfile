FROM ubuntu:latest

RUN echo "deb http://mirrors.163.com/ubuntu/ bionic main restricted universe multiverse" > /etc/apt/sources.list \
	&& echo "deb http://mirrors.163.com/ubuntu/ bionic-security main restricted universe multiverse" >> /etc/apt/sources.list \
	&& echo "deb http://mirrors.163.com/ubuntu/ bionic-updates main restricted universe multiverse" >> /etc/apt/sources.list \
	&& echo "deb http://mirrors.163.com/ubuntu/ bionic-proposed main restricted universe multiverse" >> /etc/apt/sources.list \
	&& echo "deb http://mirrors.163.com/ubuntu/ bionic-backports main restricted universe multiverse" >> /etc/apt/sources.list \
	&& echo "deb-src http://mirrors.163.com/ubuntu/ bionic main restricted universe multiverse" >> /etc/apt/sources.list \
	&& echo "deb-src http://mirrors.163.com/ubuntu/ bionic-security main restricted universe multiverse" >> /etc/apt/sources.list \
	&& echo "deb-src http://mirrors.163.com/ubuntu/ bionic-updates main restricted universe multiverse" >> /etc/apt/sources.list \
	&& echo "deb-src http://mirrors.163.com/ubuntu/ bionic-proposed main restricted universe multiverse" >> /etc/apt/sources.list \
	&& echo "deb-src http://mirrors.163.com/ubuntu/ bionic-backports main restricted universe multiverse" >> /etc/apt/sources.list \
	&& apt-get update \
    && apt-get install -y curl iputils-ping net-tools netcat tcpdump mysql-server vim \
    && mkdir /var/run/mysqld \
    && sed -i 's/^user\s\+=\s\+mysql/user = root/' /etc/mysql/mysql.conf.d/mysqld.cnf
