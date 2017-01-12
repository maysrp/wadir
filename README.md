# wadir



### Aria2 安装:

Debian 8系统 apt-get 安装
 
``` 
apt-get update && apt-get install -y aria2 
```

创建目录: 

```
mkdir /root/.aria2 
```

修改配置文件: 下载配置文件:http://webdir.cc/aria2.conf 

修改配置信息请参考:<a href="http://aria2c.com/usage.html">aria2.conf</a>

保存到刚刚的目录上 

```
wget http://webdir.cc/aria2.conf /root/.aria2/ 
```

下载http://webdir.cc/dht.dat dht.dat 到/root/.aria2/ 
```
wget http://webdir.cc/dht.dat /root/.aria2/ 
```
执行命令: 
```
echo '' > /root/aria2.session 
```
执行命令，让aria2启动: 
若没安装screen 请先
```
apt-get install -y screen 
```

在安装好screen后执行
```
screen -dmS aria2 aria2c --enable-rpc --rpc-listen-all=true --rpc-allow-origin-all -c 
```

### index.php

将你的文件按放入你的网站目录即可;


#### 配置
密码:
```
define("PASS", "admin");
```
配置显示文件以及文件夹
```
$this->notex=array("php","js","tgz");//不允许显示的后缀名文件
$this->notdir=array("a","phpmyadmin");//不允许显示的文件夹
```

![bt1.png](http://inory.net/images/2016/12/26/bt1.png)



![1561515.png](http://inory.net/images/2017/01/03/1561515.png)


![9a0d9c0ad93e4577.png](http://inory.net/images/2016/12/22/9a0d9c0ad93e4577.png)



