# DMS Java SDK示例<a name="sdk_01_0028"></a>

分布式消息服务（Distributed Message Service）是一项基于高可用分布式集群技术的消息中间件服务，具有大规模、高可靠、高并发访问、可扩展且完全托管的特点。DMS帮助云端的应用程序组件去耦合，具有很高的成本效益。

## 创建队列<a name="section2519576511428"></a>

下面代码为消息队列的创建，创建成功后，可往此队列上生产消息，使用示例：

```
String name = randomName();
String description = "sdk-unittest"
Queue queue = null;
queue = osclient.messageQueue().queue().create(name, description);
```

## 创建消费组<a name="section5273677014726"></a>

下面代码为消费组的创建，创建成功后该消费组可消费队列上的消息，使用示例：

```
List<ConsumerGroup> groups = null;
List<String> groupNames = Lists.newArrayList("consumer-group-1", "consumer-group-2");
queueId queueID = queue.getId();
groups = osclient.messageQueue().consumerGroups().create(queueID, groupNames);
```

## 生产消息<a name="section664951271485"></a>

下面代码为生产消息的过程，使用示例：

```
public void testProduceMessage() {
HashMap<String, Object> attributes1 = Maps.newHashMap();
attributes1.put("attr1", 1);
attributes1.put("attr2", false);
QueueMessage message = QueueMessage.builder().body("sdk-unittests").attributes(attributes1).build();
ActionResponse produce = osclient.messageQueue().messages().produce(queue.getId(), message);
}
```

## 消费消息<a name="section2625843514831"></a>

下面代码为消费消息的过程，使用示例：

```
public void testConsumeMessages() {
ConsumerGroup consumerGroup1 = groups.get(0);
List<QueueMessageWithHandler> all = Lists.newArrayList();
for (int i = 0; i < 3; i++) {
List<QueueMessageWithHandler> temp = osclient.messageQueue().messages().consume(queue.getId(), consumerGroup1.getId(), 5, 10);
all.addAll(temp);
}
}
```

