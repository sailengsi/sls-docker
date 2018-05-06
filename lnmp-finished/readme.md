# 使用步骤

## 导入镜像

- docker load --input sailengsi-centos-lnmp-org-v1.5.tar

## 启动容器

- docker-compose up -d

## 查看容器ID

- docker ps -a

## 对MySQL，PHP，Nginx做数据持久化

- docker cp CONTAINER_ID:/usr/local/mysql mysql
- docker cp CONTAINER_ID:/usr/local/php php
- docker cp CONTAINER_ID:/usr/local/nginx nginx

## 重启容器

- docker-compose down
- docker-compose up -d

## 启动lnmp服务

- docker-compose exec CONTAINER_ID bash
- lnmp start

## 测试

打开宿主机浏览器，访问localhost，看是否能看到lnmp.org安装包完成之后的熟悉的界面。

## 问题

执行 `docker-compose up -d`时，请确保本地端口`80`没有被占用，否则启动不成功，如果不使用80端口，可以在修改此目录内`docker-compose.yml`中的`ports`即可。
