# 图书管理系统

## 项目综述
本项目基于visual C++开发，主要功能有添加书籍，删除书籍，查找图书位置，查询图书借阅情况，借书还书等。
## 项目示例
***<label style=color:#008080;font-size:20px>菜单栏***
```C++
        cout << "图书管理系统" << endl;
        cout << "1.添加图书" << endl;
        cout << "2.删除图书" << endl;
        cout << "3.查找图书位置" << endl;
        cout << "4.查找图书借还情况" << endl;
        cout << "5.退出" << endl;
```
***<label style=color:#008080;font-size:20px>载入数据库***
```C++
MYSQL mysql;
    mysql_init(&mysql);
    if (!(mysql_real_connect(&mysql, "localhost", "root", "123456", "mysql", 0, NULL, 0))) {
        cout<<"连接失败"<<endl;
        mysql_error(&mysql);
        return 0;
    }
    mysql_query(&mysql, "set character set utf8");
```

![图书管理](http://www.qqtn.com/up/2016-1/14537772463078031.jpg)
