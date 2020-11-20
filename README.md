课室管理系统配置文档

**1.** **系统使用配置说明**

**1)**   **服务器端**

浏览器打开http://47.100.227.143，选择以下账号进行登录：

| **账号** | **密码** | **权限**                                   |
| -------- | -------- | ------------------------------------------ |
| root     | 123456   | 超级管理员（课室审批、设备审批、用户管理） |
| 5        | 123456   | 学生（申请、查询、报修）                   |

 

**2)**   **本地代码运行**

A.  安装python 3以上版本；

B.  安装pip工具；

C.  命令行执行pip install django，安装django；

D.  解压进入程序包目录，命令行运行python manage.py runserver；

E.  浏览器进入localhost:8000，选择以下账号进行登录：

| **账号** | **密码** | **权限**           |
| -------- | -------- | ------------------ |
| sa       | sa       |设备管理员（同上） |
| 10000       | 20202020       |超级管理员（同上） |
| 16369058 | 123456   | 学生（同上）       |

 

**2.** **其他说明（重要）**

推荐使用服务器端测试系统，上面有较多的测试数据展示；

由于腾讯邮箱权限设置问题，邮箱验证功能可能无法正常使用；

本地数据库文件是sqlite3.db，放在顶层目录中，没有用户名和密码，直接可以访问（项目的配置文件是位于MIS/settings.py）；

具体功能实现函数参考本地代码。