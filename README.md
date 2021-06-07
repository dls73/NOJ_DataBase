# NOJ_DataBase
南京邮电大学数据库课程实验：实现简单的图书馆数据库管理系统

## 所需软件环境
SQL Server2008 数据库工具开发版（中文版）   

## 功能要求
完成一个简易的数据库管理系统，该系统具有读者和图书的，借、还等管理功能。    

1、设计三张表分别记录读者、图书和借阅信息。每本书只有一本，每个读者借阅时间为一个月并且针对借阅权限不做限制。   

2、创建触发器和存储过程进行借、还书操作。    

1）针对借阅信息表的插入操作创建触发器，当借阅信息表进行插入操作时，自动根据书号，将图书信息表相应记录的“状态”字段发生变化。    

2）针对借阅信息表的删除操作创建触发器，当借阅信息表进行删除操作时，自动根据书号，将图书信息表相应记录的“状态”字段发生变化。    

3）创建存储过程实现借书功能即：向借阅信息表进行插入操作，将书号、借书证号，借书时间作为参数，并自动的将还书时间设置为借书时间后一个月。    

4）创建存储过程现实还书功能即：根据书号对借阅信息表进行删除操作，将书号作为参数。    