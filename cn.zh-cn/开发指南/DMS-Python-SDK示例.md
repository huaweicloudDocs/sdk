# DMS Python SDK示例<a name="sdk_02_0029"></a>

分布式消息服务（Distributed Message Service）是一项基于高可用分布式集群技术的消息中间件服务，具有大规模、高可靠、高并发访问、可扩展且完全托管的特点。DMS帮助云端的应用程序组件去耦合，具有很高的成本效益。

## 创建队列<a name="section647023214146"></a>

下面代码为消息队列创建的过程，创建成功后，可在此队列上生产消息，示例：

```
queue_dict = {
                'name': "dmsTestQueue" + self.timeStamp,
                'description': "dmsTestQueue" + self.timeStamp
}
q = conn.dms.create_queue(**queue_dict)
```

## 创建消费组<a name="section28983774141434"></a>

下面代码为消费组创建的过程，创建完成后，新创建的消费组，可消费队列上的消息，示例：

```
groupDict = {
            "groups": [
                {
                    "name": "dmsConsumeGroup" + self.timeStamp
                }
            ]
 }
group = conn.dms.create_groups(queue, **groupDict)
```

## 生产消息<a name="section58028226142340"></a>

下面代码为生产消息的过程，示例：

```
msgDict = {
            "messages": [
                {
                    "body": "testMsg" + self.timeStamp,
                    "attributes":
                    {
                        "attribute1": "value1",
                        "attribute2": "value2"
                    }
                }
            ]
 }
conn.dms.send_messages(queue, **msgDict))
```

## 消费消息<a name="section17658960142740"></a>

下面代码为消费消息的过程，示例：

```
msgList =  conn.dms.consume_message(queue, group[0].id)
```

