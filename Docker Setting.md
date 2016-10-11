# Docker Mac os x Install

1,安装Docker

$ brew cask install virtualbox
$ brew install docker
$ brew install docker-machine

2，Docker安装版本确认

$ virtualbox --help
$ docker -v
$ docker-machine -v

3，虚拟机作成

$ docker-machine create --driver virtualbox test-docker

4，虚拟机确认

$ docker-machine ls

5，虚拟机状态确认

$ docker-machine status test-docker

6，SSH虚拟机

$ docker-machine ssh test-docker

7，下载Image

$ docker pull centos:7

8，Image确认

$ docker images

9，创建Container（不启动）

$ docker create -it --name centos7 centos:7

10，创建并启动Container

$ docker run -it --detach --name centos7.01 centos:7

11，Container确认

$ docker ps -a

2016年10月12日 00:55
