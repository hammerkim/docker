# docker-centos-7
## 

##### 1. Add package
+ wget
+ net-tools
##### 2. enable systemd command


## Docker build
docker build --rm -t hammerkim/centos7-systemd:0.1 .


## Docker run
docker run --privileged -itd -e container=docker \
      --name centos7-systemd \
      -v /sys/fs/cgroup:/sys/fs/cgroup:ro \
      hammerkim/centos7-systemd:0.1 
      /usr/sbin/init

+ -v /sys/fs/cgroup:/sys/fs/cgroup:ro
+ /usr/sbin/init