# MRS Java SDK示例<a name="sdk_01_0029"></a>

MapReduce服务（MapReduce Service）：提供租户完全可控的企业级大数据集群云服务，轻松运行Hadoop、Spark、HBase、Kafka、Storm等大数据组件。

## 创建集群并提交作业<a name="section15025863192851"></a>

下面代码为MRS集群创建并提交作业的过程，用户可以根据需求进行相应的参数配置，创建完成后，新创建的集群会在MRS服务的集群列表页面上显示。

```
public void createClusterAndRunAJob() 
{
MapReduceComponent component = MapReduceComponent.builder().id(component_id).name(component_name).version(component_version).desc(component_desc).build();
MapReduceClusterCreate cluster = MapReduceClusterCreate.builder().dataCenter(data_center).masterNodeNum(master_node_num).masterNodeSize(master_node_size).coreNodeNum(core_node_num).coreNodeSize(core_node_size).name(cluster_name).availablilityZoneId(available_zone_id).vpcName(vpc).vpcId(vpc_id).subnetName(subnet_name).subnetId(subnet_id).version(cluster_version).type(cluster_type).volumeSize(volume_size).volumeType(volume_type).keypair(node_public_cert_name).safeMode(safe_mode).components(Lists.newArrayList(component)).build();
MapReduceJobExeCreate jobExe = MapReduceJobExeCreate.builder().jobType(job_type).jobName(job_name).jarPath(jar_path).arguments(arguments).input(input).output(output).jobLog(job_log).fileAction(file_action).hql(hql).hiveScriptPath(hive_script_path).shutdownCluster(shutdown_cluster).submitJobOnceClusterRun(submit_job_once_cluster_run).build();
MapReduceClusterCreateResult result = osclient.mrs().clusters().createAndRunJob(cluster, jobExe);
}
```

## 查询集群详情<a name="section52473016193537"></a>

下面代码为查询集群详情的过程，用户需要传入集群id。

```
public void describeCluster () {
MapReduceClusterInfo cluster = osclient.mrs().clusters().get(id);
}
```

## 终止集群<a name="section692608019378"></a>

下面代码为查询集群详情的过程，用户需要传入集群id。

```
public void deleteCluster () {
ActionResponse delete = osclient.mrs().clusters().delete(id);
}
```

## 新增作业并执行<a name="section46585772193825"></a>

下面代码为新增作业并执行的过程，用户可以根据需求进行相应的参数配置，创建完成后，新创建的作业会在MRS服务的作业列表页面上显示。

```
public void submitAndExecuteJob () {
MapReduceJobExeCreate jobExeCreate = MapReduceJobExeCreate.builder().jobType(job_type).jobName(job_name).clusterId(cluster_id).jarPath(jar_path).arguments(arguments).input(input).output(output).jobLog(job_log).fileAction(file_action).hql(hql).hiveScriptPath(hive_script_path).isProtected(is_protected).isPublic(is_public).build();
MapReduceJobExe exe = osclient.mrs().jobExes().create(jobExeCreate);
}
```

## 查询作业exe对象列表<a name="section61046302193938"></a>

下面代码为查询作业exe对象列表的过程，用户可以根据需求进行相应的参数配置。

```
public void getJobExeList () {
JobExeListOptions options = JobExeListOptions.create().page(current_page).pageSize(page_size).clusterId(cluster_id)
.state(state);
List<? extends MapReduceJobExe> list = osclient.mrs().jobExes().list(options);
}
```

## 查询作业exe对象详情<a name="section22865048194039"></a>

下面代码为查询作业exe对象详情的过程，用户需要传入作业exe对象id。

```
public void getJobExes() {
osclient.mrs().jobExes().get(id);
}
```

## 删除作业执行对象<a name="section42506813194136"></a>

下面代码为删除作业执行对象详情的过程，用户需要传入作业执行对象id。

```
public void deleteJobExecution () {
ActionResponse delete = osclient.mrs().jobExecutions().delete(id);
}
```

