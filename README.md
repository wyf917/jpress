
## JPress 官网

http://www.jpress.io

## JPress 文档 

[点击这里](./doc/readme.md)

## JPress School 

https://mp.weixin.qq.com/s/GbNv0xaK6jruWqTDJ_Ospw

    
## 新版本相关视频教程

* **1. JPress下载、编译、运行** 

https://pan.baidu.com/s/1Pe0KcYcQGalxPnlUNw9rmg

* **2. 一个小时开发一个论坛**

https://pan.baidu.com/s/1rJ5OMOxUwVz9ylK3oFD3PQ

* **3. JPress模板开发教程**

https://pan.baidu.com/s/1zSSezfMOfrZxGvs_Sz4Kig  密码:tvzh

* **4. JPress与CDN的整合实现**

https://pan.baidu.com/s/10aPgdD1HNZO1qb5ab9YB5w

## JPress 微信小程序SDK

网址：https://gitee.com/fuhai/jpress-miniprogram-sdk

## 通过Docker运行JPress

##### 1、安装docker

过程略

##### 2、通过docker-compose 运行 JPress

Linux :

```
wget https://gitee.com/fuhai/jpress/raw/master/docker/docker-compose.yml
docker-compose up -d
```

Mac OS :

```
curl -O https://gitee.com/fuhai/jpress/raw/master/docker/docker-compose.yml
docker-compose up -d
```

然后访问 127.0.0.1:8080 ，JPress会引导安装过程，一路下一步就可以了。

停止JPress ：

```
docker-compose stop
```

再次启动JPress：

```
docker-compose start
```


## 常见问题

#### 问题1： 如何在运行JPress ？

如果使用Docker，以上已经给出了方法。

如果是tomcat，下载源码，通过 `mvn clean install`命令之后，在 `stater-tomcat/target` 目录下回生成 jpress 的war包。把war包扔到自己对他tomcat，并启动tomcat即可。

JPress会引导你走安装过程。

#### 问题2：如何导入 idea 或 eclipse 开发工具运行

分为以下几步：

1. 通过maven的方式导入到 idea 或 eclipse
2. 在 `starter` 的 resource 目录下创建文件 jboot.properties 和 install.lock 文件
3. 通过 jpress 根目录下的 `db-init.sql` 初始化数据库
4. 运行 `starter` 下的 DevStarter.java 的 `main()` 方法即可

**说明：**

* jboot.porperties ：jpress 主要的配置文件（重命名 `jboot-simple.properties` 为 `jboot.properties` ，并修改其数据库连接等信息）
* install.lock ：如果没有该文件，jpress会自动安装。空白内容即可。



#### 问题3：为什么运行不起来?

注意下你本地的环境，JPress要求的环境如下：

* jdk: 1.8.x
* tomcat: 8.x
* mysql: 5.6+

#### 问题4：为什么无法对文章进行评论

答：JPress的文章评论功能默认是关闭的，请先在后台 `文章 -> 设置` 开启评论功能。


**更多问题，请关注 JPress 公众号 ：**

![](./doc/images/jpress_qrcode.jpg)


**JPress后台截图**

![](./doc/images/screenshot/001.png)

![](./doc/images/screenshot/002.png)

![](./doc/images/screenshot/003.png)

![](./doc/images/screenshot/004.png)

![](./doc/images/screenshot/005.png)

![](./doc/images/screenshot/006.png)

![](./doc/images/screenshot/007.png)

![](./doc/images/screenshot/008.png)

![](./doc/images/screenshot/009.png)

![](./doc/images/screenshot/010.png)

![](./doc/images/screenshot/011.png)

![](./doc/images/screenshot/012.png)

![](./doc/images/screenshot/013.png)

**用户中心的相关截图**

![](./doc/images/screenshot/014.png)

![](./doc/images/screenshot/015.png)

![](./doc/images/screenshot/016.png)

![](./doc/images/screenshot/017.png)



