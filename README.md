# mongo-express

mongo-express是使用Node.js和express实现的轻量级MongoDB管理程序，通过它您可以轻松管理您存储在MongoDB的数据。

## 注意事项

目前该mongo-express镜像不支持授权认证，您启动mongo-express容器后，容器的URL是公开访问的。所以，您使用完毕后请立即“停止”容器，防止MongoDB数据被他人操作。

## 版本

0.20.0

## 使用说明

* 从最新镜像启动mongo-express容器
* 绑定一个需要管理的MongoDB服务实例，设置服务别名为“MongoDB”（绑定时的默认值）
* 启动容器