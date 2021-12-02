1.阿里云安装mysql

```shell
sudo dnf install @mysql

```





2.mysql登陆

```shell
mysql -uroot -p
```



3.设置防火墙

```shell
iptables -A INPUT -m state --state NEW -m tcp -p tcp --dport 3306 -j ACCEPT
```