# Woodpecker
运维三件套，跳板机，发布系统，mysql审核系统
##简介
做为一个运维，工具太多，但是又不得不使用，那就从源头进行合并吧。这里把运维的三个主要工具进行合并，可能会用到源码，也可能用不到源码。本人主要是为了学习一些相关语言的知识点所以才做的这个系统，可能有不足的地方，不过在后期的版本更新中慢慢的进行完善。如有需求，可以关注后期的更新。
##功能特性
1、实现远程访问，通过跳板机利用用户名或密钥
- 通过跳板机访问远程服务
- 远程数据上传和下载
- 用户操作记录

2、实现发布系统，利用用户名或密钥
- 在不影响用户请求的前提下发布应用
- 发布过程中实时打印日志，打印日志行数可以设置
- 自动设置slb或者对nginx的upstreams增删操作

3、通过审核更新mysql数据，利用用户名和密码操作
- 最多三个等级
- 第一等级用户向第二等级用户申请，第二等级用户审批后，第一等级方可操作
- 第一等级申请后，执行针对申请的操作方可执行
- 管理员可以设置用户组申请的权限：读、写、更新
