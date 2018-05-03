# armhf-alpine-mysql
a docker image base on armhf-alpine with mysql

works fine at armhf linux,x-pi

# build image
```
docker build -t erlgos/mysql .
docker run -it --rm -v $(pwd):/app -p 3306:3306 erlgos/mysql
```

# Usage
```
docker run -it --name mysql -p 3306:3306 -v $(pwd):/app -e MYSQL_DATABASE=admin -e MYSQL_USER=tony -e MYSQL_PASSWORD=dpa\*12d -e MYSQL_ROOT_PASSWORD=111111 wangxian/alpine-mysql
```

It will create a new db, and set mysql root password(default is 111111)
