# FishChatServer2

说明
======
吸取了第一版的经验以及我们商业版的探索。第二版我更多的思考在不要过多的实现轮子，这个版本将很多业务无关的代码去掉，
全面拥抱`Kubernetes + Docker + grpc` 来实现业务之下的东西。并且尽量靠拢`微服务`。

架构
======

协议
======
在`protocol`目录下

```shell
external 是对外的协议，采用`protobuf`实现
rpc 是服务内部的调用，采用`grpc`

```

部署
======
