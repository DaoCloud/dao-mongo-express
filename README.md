# Mongo Express

Mongo Express 是使用 Node.js 和 Express 框架实现的轻量级 MongoDB 数据库管理程序，通过它您可以轻松管理您的 MongoDB 数据库。

## 注意事项

目前在 DaoCloud 镜像仓库提供的 Mongo Express 版本不支持授权认证，您启动 Mongo Express 容器后，容器的 URL 是公开访问的。所以在您使用完毕后请立即「停止」容器，防止 MongoDB 数据库被他人操作。

## 版本

0.20.0

## 如何使用这个镜像管理 DaoCloud MongoDB 服务

* 从最新镜像启动 mongo-express 容器。
* 绑定一个需要管理的 MongoDB 服务实例，设置服务别名为「MongoDB」（不区分大小写）。
* 启动容器。

## 如何使用这个镜像管理我自己的 MongoDB 数据库

这个镜像在启动时依赖于下面几个环境变量来配置 MongoDB 数据库连接

* 「**MONGODB_PORT_27017_TCP_ADDR**」  MongoDB 数据库 IP
* 「**MONGODB_PORT_27017_TCP_PORT**」  MongoDB 数据库端口
* 「**MONGODB_INSTANCE_NAME**」  MongoDB 数据库名称
* 「**MONGODB_USERNAME**」  MongoDB 数据库用户名
* 「**MONGODB_PASSWORD**」  MongoDB 数据库密码
