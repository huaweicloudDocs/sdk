# MRS Python SDK示例<a name="ZH-CN_TOPIC_0079299145"></a>

MapReduce服务（MapReduce Service）：提供租户完全可控的企业级大数据集群云服务，轻松运行Hadoop、Spark、HBase、Kafka、Storm等大数据组件。

## 创建集群并提交作业<a name="section159681309145"></a>

下面代码为MRS集群创建并提交作业的过程，用户可以根据需求进行相应的参数配置，创建完成后，新创建的集群会在MRS服务的集群列表页面上显示。

```
vpc_id = vpc_id
vpc_name = vpc_name
subnet_id = subnet_id
subnet_name = subnet_name
keypair_name = keypair_name

cluster = {
"cluster_name": cluster_name,
"billing_type": billing_type,
"data_center": data_center,
"master_node_num": master_node_num,
"master_node_size": master_node_size,
"core_node_num": core_node_num,
"core_node_size": core_node_size,
"available_zone_id": available_zone_id,
"vpc": vpc,
"vpc_id": vpc_id,
"subnet_id": subnet_id,
"subnet_name": subnet_name,
"cluster_version": cluster_version,
"cluster_type": cluster_type,
"volume_type": volume_type,
"volume_size": volume_size,
"keypair": keypair,
"safe_mode": safe_mode,
"component_list": [{
"component_id": component_id,
"component_name": component_name
}]
}

job = {
"job_type": job_type,
"job_name": job_name,
"jar_path": jar_path,
"arguments": arguments,
"input": input,
"output": output,
"job_log": job_log,
"shutdown_cluster": shutdown_cluster,
"file_action": file_action,
"submit_job_once_cluster_run": submit_job_once_cluster_run,
"hql": hql,
"hive_script_path": hive_script_path
}
cluster = conn.map_reduce.create_cluster_and_run_job(cluster, job)
```

## 扩容集群节点<a name="section6488255191927"></a>

下面代码为扩容集群节点的过程，用户需要传入集群id。

```
expand_node_amount = instances
conn.map_reduce.expand_cluster(id, expand_node_amount)
```

## 查询集群详情<a name="section3974245492111"></a>

下面代码为查询集群详情的过程，用户需要传入集群id。

```
cluster = conn.map_reduce.get_cluster(id)
```

## 终止集群<a name="section596420492218"></a>

下面代码为查询集群详情的过程，用户需要传入集群id。

```
conn.map_reduce.delete_cluster(id)
```

## 新增作业并执行<a name="section5001869492358"></a>

下面代码为新增作业并执行的过程，用户可以根据需求进行相应的参数配置，创建完成后，新创建的作业会在MRS服务的作业列表页面上显示。

```
exe = {
"job_type": job_type,
"job_name": job_name,
"cluster_id": cluster_id,
"jar_path": jar_path,
"arguments": arguments,
"input": input,
"output": output,
"job_log": job_log,
"file_action": file_action,
"hql": hql,
"hive_script_path": hive_script_path
}
job_exe = conn.map_reduce.exe_job (**exe)
```

## 查询作业exe对象列表<a name="section5458598292831"></a>

下面代码为查询作业exe对象列表的过程，用户可以根据需求进行相应的参数配置。

```
query = {
"cluster_id": cluster_id,
"job_name": job_name,
"page_size": page_size,
"current_page": current_page,
"state": state
}
executions = list(conn.map_reduce.job_exes(**query))
```

## 查询作业exe对象详情<a name="section5475582292953"></a>

下面代码为查询作业exe对象详情的过程，用户需要传入作业exe对象id。

```
conn.map_reduce.get_job_exe(id)
```

## 删除作业执行对象<a name="section31114389313"></a>

下面代码为删除作业执行对象详情的过程，用户需要传入作业执行对象id。

```
conn.map_reduce.delete_job_execution(id)
```

