# 常规问题排查方法

## 1.查看日志

**mobileark日志路径**：/home/mobileark/mobileark/tomcat/logs/catalina.out

**exmobi日志路径**：/home/exmobi/exmobi/tomcat/logs/catalina.out

**mos日志路径**：/home/mos/mos/tomcat/logs/catalina.out

**nginx**：/usr/local/nginx/logs/access.log

## 2.查看进程

**mobileark**：ps -ef | grep mobileark

**exmobi**：ps -ef | grep exmobi

**mos**：ps -ef | grep mos

**redis**：ps -ef | grep redis

## 3.查看端口

netstat -anpl | grep 端口

## 4.判断网络是否正常

telnet ip port，如：telnet 192.168.100.1 8080

ping ip，如：ping 192.168.100.0

curl，如：curl http://192.168.100.1/file/test.doc

## 5.mobileark模块相关

**程序安装路径**：/home/mobileark/mobileark

**应用路径**：/var/empdata/data/resources/application/

**头像路径**：/var/empdata/data/resources/useravatar/

**同步插件路径**：/var/empdata/data/resources/ldap/

**数据库配置文件路径**：/home/mobileark/mobileark/tomcat/conf/context.xml

**redis配置文件路径**：/home/mobileark/mobileark/mobileark/WEB-INF/classes/redis.properties

## 6.exmobi模块相关

**程序安装路径**：/home/exmobi/exmobi/

**应用路径**：/home/exmobi/exmobi/data/emp/resources/

**DCS文件缓存路径**：/var/empdata/data/resources/useravatar/

**PNS推送证书路径**：/home/exmobi/exmobi/data/pns/apnscertificate/

**数据库配置文件路径**：/home/exmobi/exmobi/exmobi/WEB-INF/classes/jdbc.properties

## ７.服务器常规检查

查看操作系统版本：cat /etc/redhat-release

查看操作系统位数：uname -a

查看系统内存情况：free -m

查看磁盘情况：df -h

查看jdk版本：java -version

