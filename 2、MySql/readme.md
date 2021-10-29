# MySql

常见指令

- mysql -u root -p 进入mysql命令交互
- mysqkd --install  将mysql假如到windows的服务中
- mysqld --initialize --user=root --console 初始化mysql数据
- net start mysql 启动mysql
- net stop mysql 停止mysql
- set password = '123456'; 修改密码为123456

> 链接地址：
https://blog.csdn.net/m0_37987151/article/details/84316008


show variables like 'character\_set\_%';  查看当前数据库字符编码

修改my.ini文件中的默认字符编码

service mysqld restart

show databases  查看当前拥有的数据库

exit; 停止;

## SQL分支

- DDL： 数据定义语言 操作数据库对象： 库、 表、 视图、 存储过程
- DML： 数据操作语言  操作数据库中的记录
- DCL:  数据控制语句 操作用户权限

create database test;
use test;
DROP DATABASE test;

<!-- 添加列 -->
alter table `test`.`student`
add column `phone` varchar(11) null after `sex`

<!-- 连接外键 -->
add foreign key (`classId`) references `test`.`class`(`id`);

## SQL的增删改查
