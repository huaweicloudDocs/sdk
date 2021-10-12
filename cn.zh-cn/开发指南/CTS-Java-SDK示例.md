# CTS Java SDK示例<a name="sdk_01_0023"></a>

## Tracker<a name="section2923193117411"></a>

云审计服务开通后系统会创建一个追踪器，用来关联系统记录的所有操作。

## 创建Tracker<a name="section2724033917204"></a>

下面代码为创建Tracker的过程，用户可以根据需求进行相应的参数配置，目前只能创建一个Tracker:“system”。

```
public void CreateTracker() { 
Tracker create = osclient.cloudTraceV1().trackers().create(bucket_name,FilePrefixName); 
}
```

## 删除Tracker<a name="section29972710172014"></a>

下面代码为删除Tracker的过程。

```
public void DeleteTraker() {
ActionResponse delete = osclient.cloudTraceV1().trackers().delete(tracker_name);
Assert.assertTrue(delete.isSuccess());
List<Tracker> trackers = osclient.cloudTraceV1().trackers().list();
Assert.assertTrue(trackers.size() == 0);
}
```

## 更新Tracker<a name="section12048274172022"></a>

下面代码为更新Tracker的过程，可以更新的信息包括桶名，文件夹名称以及status，tracker\_name可选，但只能为system。

```
public void UpdateTraker() { 
TrackerUpdate update = TrackerUpdate.builder().trackerName(tracker_name) 
.bucketName(bucket_name).filePrefixName("SDK-unittest").status(TrackerStatus.Enabled”).build(); 
Tracker updated = osclient.cloudTraceV1().trackers().update(update); 
}
```

## 查询Tracker<a name="section27381313172034"></a>

下面代码为查询Tracker的过程，参数为tracker\_name。

```
public void GetTraker() {
Tracker get = osclient.cloudTraceV1().trackers().get(tracker_name);
}
```

## Trace<a name="section1957093017625"></a>

通过事件查询接口，可以查处系统记录的7天内资源操作记录。

## 查询Trace列表<a name="section43893880172044"></a>

下面代码为查询trace列表，可以设置多个查询参数进行筛选。

```
/*v2interface*/
publicvoidListTrace(){
	TraceListOptionsoptions=TraceListOptions.create().limit(5).user("renxiaomei").serviceType("CTS");
	List<Trace>list=osclient.cloudTraceV2().traces().list("system", options);
	if(list.size()>0){
		Tracetrace=list.get(list.size()-1);
		options.marker(trace.getId());
		List<Trace>list2=osclient.cloudTraceV2().traces().list("system", options);
	}
}
```

