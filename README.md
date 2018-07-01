# [Docker](http://www.docker.org.cn/book/docker/what-is-docker-16.html)

## 搜索可用镜像
> docker search tutorial

## 下载容器镜像
> docker pull learn/tutorial

## 在docker容器中运行hello world!
> docker run learn/tutorial echo "hello world"

## docker run 停止后自动删除该容器; 用于测试时好用
> docker run --name mysql --rm -p 3306:3306 -e MYSQL_ROOT_PASSWORD=root -dit mysql

## 在容器中安装新程序
> docker run learn/tutorial apt-get install -y ping

## 保存对容器的修改
> docker commit [容器 id] pengminmin/ping

## 运行新的镜像
> docker run pengminmin/ping www.baidu.com

## 检查运行中的镜像
> docker inspect [容器 id]

## 发布自己的镜像
> docker push pengminmin/ping
