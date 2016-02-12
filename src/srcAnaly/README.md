# 关系查询处理器
一个关系查询处理器以一个SQL语句作为输入,然后进行验证,优化成为一个程序数据流执行计划,并且在获得准入许可以后可以代表一个客户程序执行数据流程序.接着,客户程序获取元组,通常一次一个元组或一小批元组.<br><br>
在该部分内容中,我们关注查询处理器和"存储管理器访问方法的非事务处理方面".<br><br>
在本章中,我们将重点放在常见的SQL命令:数据操作语言(DML)语句包括SELECT、INSERT、UPDATE和DELETE.像CREATE TABLE和CREATE INDEX这样的数据定义语言(DDL)语句通常不被查询优化器处理的.这些语句通常是由静态DBMS逻辑通过调用存储引擎和目录管理器来实现的.