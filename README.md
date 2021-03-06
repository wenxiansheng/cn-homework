# cn-homework
## [第一周](https://github.com/wenxiansheng/cn-homework/blob/main/week-01/main.go)
课后练习 1.1
编写一个小程序：
给定一个字符串数组
[“I”,“am”,“stupid”,“and”,“weak”]
用 for 循环遍历该数组并修改为
[“I”,“am”,“smart”,“and”,“strong”]

课后练习 1.2
基于 Channel 编写一个简单的单线程生产者消费者模型：

队列：
队列长度 10，队列元素类型为 int
生产者：
每 1 秒往队列中放入一个类型为 int 的元素，队列满时生产者可以阻塞
消费者：
每一秒从队列中获取一个元素并打印，队列为空时消费者阻塞

## [第二周](https://github.com/wenxiansheng/cn-homework/blob/main/week-02/main.go)
1. 接收客户端 request，并将 request 中带的 header 写入 response header
2. 读取当前系统的环境变量中的 VERSION 配置，并写入 response header
3. Server 端记录访问日志包括客户端 IP，HTTP 返回码，输出到 server 端的标准输出
4. 当访问 localhost/healthz 时，应返回 200

## [第三周](https://github.com/wenxiansheng/cn-homework/blob/main/week-03/Dockerfile)
1. 构建本地镜像
2. 编写 Dockerfile 将练习 2.2 编写的 httpserver 容器化
3. 将镜像推送至 docker 官方镜像仓库
4. 通过 docker 命令本地启动 httpserver
5. 通过 nsenter 进入容器查看 IP 配置

目前已经push到[官方repo](https://hub.docker.com/repository/docker/liuguannyi/httpserver)
```
docker run -d -p 80:80 liuguannyi/httpserver:1.0
```