# Anti-DDoS Java SDK示例<a name="sdk_01_0027"></a>

## 查询Anti-DDoS配置可选范围<a name="section3944661591450"></a>

查询系统支持的Anti-DDoS防护策略配置的可选范围，用户根据范围列表选择适合自已业务的防护策略进行Anti-DDoS流量清洗。

代码示例如下：

```
public void listConfigs()
    {
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService=antiDDoSServices.antiddos();
        AntiDDoSConfig configs = antiDDoSService.listConfigs();
        LOGGER.info("{}", configs);
    }
```

## 开通Anti-DDoS服务<a name="section26684654172532"></a>

用户开通Anti-DDoS流量清洗防护。作为异步接口，调用成功，只是说明服务节点收到了开通请求，开通是否成功需要通过任务查询接口查询该任务的执行状态。

代码示例如下：

```
public void createAntiDDoS() throws InterruptedException
    {
        AntiDDoS entity = AntiDDoS.builder()
            .enableL7(true)
            .trafficPos(TrafficPos.POS_1)
            .httpRequestPos(HttpRequestPos.POS_1)
            .cleaningAccessPos(CleaningAccessPos.POS_1)
            .appType(AppType.Type_0)
            .build();
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService =antiDDoSServices.antiddos();
        Task task = antiDDoSService.create(entity, floatingIpId);
        LOGGER.info("{}", task);
        taskId = task.getTaskId();
        waitTaskFinish(taskId);    }
   }
}
```

## 关闭Anti-DDoS服务<a name="section27490877172539"></a>

用户关闭Anti-DDoS流量清洗防护。作为异步接口，调用成功，只是说明服务节点收到了关闭防护请求，操作是否成功需要通过任务查询接口查询该任务的执行状态。

代码示例如下：

```
public void deleteAntiDDoS()
        throws InterruptedException
    {
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService=antiDDoSServices.antiddos();
        Task task = antiDDoSService.delete(floatingIpId);
        LOGGER.info("{}", task);
        waitTaskFinish(task.getTaskId());
}
```

## 查询Anti-DDoS服务<a name="section13330669172546"></a>

查询配置的Anti-DDoS防护策略，用户可以查询指定EIP的Anti-DDoS防护策略。

代码示例如下：

```
public void getAntiDDoS()
    {
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService =antiDDoSServices.antiddos();
        AntiDDoS antiDDoS = antiDDoSService.get(floatingIpId);
        LOGGER.info("{}", antiDDoS);
    }
```

## 更新Anti-DDoS服务<a name="section11656122172548"></a>

更新指定EIP的Anti-DDoS防护策略配置。调用成功，只是说明服务节点收到了更新配置请求，操作是否成功需要通过任务查询接口查询该任务的执行状态。

代码示例如下：

```
public void updateAntiDDoS() throws InterruptedException
    {
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService =antiDDoSServices.antiddos();
        AntiDDoS entity = antiDDoSService.get(floatingIpId);
        entity = entity.toBuilder().appType(AppType.Type_1).build();
        Task task = osclient.antiDDoS().antiddos().update(entity, floatingIpId);
        LOGGER.info("{}", task);
        waitTaskFinish(task.getTaskId());
    }
```

## 查询Anti-DDoS任务<a name="section24002378172550"></a>

用户查询指定的Anti-DDoS防护配置任务，得到任务当前执行的状态。

代码示例如下：

```
public void getTask()
    {
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService =antiDDoSServices.antiddos();
        Task task = antiDDoSService.getTask(taskId);
        LOGGER.info("{}", task);
}
```

## 查询EIP防护状态列表<a name="section4361571172552"></a>

查询用户所有EIP的Anti-DDoS防护状态信息，用户的EIP无论是否绑定到云服务器，都可以进行查询。

代码示例如下：

```
public void listStatuses()
{
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService =antiDDoSServices.antiddos();
        AntiDDoSStatus statuses = antiDDoSService.listStatus();
        LOGGER.info("{}", statuses);
}
```

## 查询指定EIP防护状态<a name="section54758667172554"></a>

查询指定EIP的Anti-DDoS防护状态。

代码示例如下：

```
public void getStatus()
    {
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService =antiDDoSServices.antiddos();
        AntiDDoSStatusDetail status = antiDDoSService.getStatus(floatingIpId);
        LOGGER.info("{}", status);
}
```

## 查询指定EIP防护流量<a name="section45228460172556"></a>

查询指定EIP在过去24小时之内的防护流量信息，流量的间隔时间单位为5分钟。

代码示例如下：

```
public void dailyReport()
    {
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService =antiDDoSServices.antiddos();
        List<? extends AntiDDoSDailyData> dailyReport = antiDDoSService.dailyReport(floatingIpId);
        LOGGER.info("{}", dailyReport);
}
```

## 查询指定EIP异常事件<a name="section9504791172557"></a>

查询指定EIP在过去24小时之内的异常事件信息，异常事件包括清洗事件和黑洞事件，查询延迟在5分钟之内。

代码示例如下：

```
public void listLog()
    {
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService =antiDDoSServices.antiddos();
        List<? extends AntiDDoSLog> logs = antiDDoSService.listLogs(floatingIpId);
        LOGGER.info("{}", logs);
        
        AntiDDoSLogListOptions options = AntiDDoSLogListOptions.create().limit(1).offset(1);
        List<? extends AntiDDoSLog> logs2 = osclient.antiDDoS().antiddos().listLogs(floatingIpId, options);
        LOGGER.info("{}", logs2);
}
```

## 查询周防护统计情况<a name="section61032237172559"></a>

查询用户所有Anti-DDoS防护周统计情况，包括一周内DDoS拦截次数和攻击次数、以及按照被攻击次数进行的排名信息等统计数据。

代码示例如下：

```
public void weeklyReport()
    {
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSService antiDDoSService =antiDDoSServices.antiddos();
        AntiDDoSWeeklyData weekly = antiDDoSService.weeklyReport();
        LOGGER.info("{}", weekly);
        
        Calendar cal = Calendar.getInstance();
        cal.add(Calendar.HOUR, -10);
        AntiDDoSWeeklyData weekly2 = osclient.antiDDoS().antiddos().weeklyReport(cal.getTime());
        LOGGER.info("{}", weekly2);
    }
```

## 查询告警配置信息<a name="section5968868717261"></a>

查询用户配置信息，用户可以通过此接口查询是否接收某类告警，同时可以配置是手机短信还是电子邮件接收告警信息。

代码示例如下：

```
public void queryWarningInfo()
    {
        AntiDDoSServices antiDDoSServices = osclient.antiDDoS();
        AntiDDoSWarn query = antiDDoSServices.warnalert().query();
        LOGGER.info("{}", query);
}
```

