# PingCAP

**Title:** 数据库研发工程师（实习）

## First-Round (2021-03-31)

- Kubernetes 架构
- `kubectl apply`
- Volcano 和 Job 的区别
  - 和 k8s 原生调度一起工作的吗？
  - 如果和原生调度在一起的话会不会出现有一些资源被原生调度器给占用了？
  - 有没有什么方法可以去规避掉这种情况？
- GitOps

## System Design

利用 mydumper 备份 MySQL 数据库到公有云对象存储上，由于 mydumper 只支持备份到本地，所以需要一个上传工具将本地备份上传到对象存储。

## Task (2021-04-02) `Suspended`

利用 mydumper 备份 MySQL 数据库到公有云对象存储上，由于 mydumper 只支持备份到本地，所以需要一个上传工具将本地备份上传到对象存储。请使用 Go 语言设计一个小工具在本地磁盘空间比较小的情况下将 MySQL 备份数据上传到 S3 类对象存储上。
