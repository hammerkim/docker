
https://hub.docker.com/r/cytopia/mariadb-10.3/

docker run -d -p 3307:3306 \
        -e  MYSQL_ROOT_PASSWORD=암호 \
        --name mariadb-10.3-centos \
        hammerkim/mariadb-10.3.22-centos:1.0