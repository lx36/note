### 1.linux下的Mysql命令

* service mysql start/stop/restart/status 

* netstat -aptn 查看当前开放端口

* systemctl status mysqld  查看mysql状态

### 2.linux 查看mysql安装位置

1. 显示软件安装地址    **whereis mysql**
2. 只查询运行文件所在地址  **which mysql**

 ### 3.ubuntu安装mysql

1. sudo apt upadate
2. sudo apt install mysql-server
3. sudo mysql_secure_installation(安全安装)



### 4.修改mysql密码

```shell
sudo vim /etc/mysql/mysql.conf.d/mysqld.cnf
# 在[mysql]下加一行 skip-grant-tables
sudo service mysql restart
mysql
use mysql;
flush privileges;
alter user 'root'@'localhost' identified by 'newpassword'
sudo vim /etc/mysql/mysql.conf.d/mysqld.cnf
# 删掉原配置
```



` ERROR 1819 (HY000): Your password does not satisfy the current policy requirements`

* 查看并修改mysql初始密码策略

   SHOW VARIABLES LIKE ‘validate_password%’;

​        set global validate_password.policy=LOW 设置密码验证强度

​        set global validate_password.length=6  设置密码长度

#### 5.windows远程连接linux上的mysql

**配置云服务器安全组，把3306端口打开**

`telnet ip port   一个用途是确定端口是否能访问        例如：telnet 120.26.0.63 3306  ` 

设置访问权限，解除本机ip地址绑定

注意防火墙的设定

```sql
use mysql;
select Host,User from user;
update user set host = '%' where user ='root'; # %是通配符，所有ip都有连接权限
flush privileges   #使配置生效


# /etc/mysql/mysql.conf.d/mysqld.cnf  mysql的配置文件
# 端口号  字符集 套接字 文件存放目录等等

# bind-address  mysql绑定的ip  默认是120.0.0.1  这样只会接受localhost的访问 #注释掉 或设为 0.0.0.0
```

