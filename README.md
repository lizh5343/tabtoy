# tabtoy


# 一些问题的处理

* 所有文件导出为1个文件

* 多文件导出时, 为了防止类型重复定义问题, 需要在全局准备一个空表导入类型信息, 其他表只是引用

行结构名称优先度从低到高来源: Sheet名->(当有多个DataSheet时)FileMeta里的TableName,  不以Sheet名来命名, 因为考虑到多Sheet时的歧义问题

Combine系统
结构体名  从命令行参数来
每个电子表格表名, 为Combine结构体的字段名, 类型为电子表格名+Define
二进制文件名  二进制路径+结构体名.bin
C#文件名  C#路径+结构体名.cs