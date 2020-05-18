# 安装Java SDK<a name="sdk_01_0004"></a>

Java SDK提供“导入Java SDK JAR文件”、“添加Maven依赖”和“从华为云镜像站下载”三种安装方式。

**方式一：**导入Java SDK JAR文件的方式，如下：

请从GitHub 上下载JAR文件，并在集成开发环境（IDE）中导入。

[https://github.com/huaweicloud/huaweicloud-sdk-release/tree/master/java-sdk](https://github.com/huaweicloud/huaweicloud-sdk-release/tree/master/java-sdk)

以Eclipse为例，创建Java工程后，执行以下步骤，导入JAR文件到新建的工程中：

1.  将下载的JAR文件复制到工程文件夹中。
2.  在Eclipse中打开工程，右键单击该项工程，选择**Properties**。
3.  在弹出的对话框中，单击**Java Build Path**，然后在**Libraries**页签下单击**Add JARs**，添加下载的JAR文件。
4.  单击**OK**。

**方式二：**添加Maven依赖的方式，如下：

通过在pom.xml文件中添加以下依赖安装Java SDK。

```
<dependency>
<groupId>com.huawei</groupId>
<artifactId>openstack4j</artifactId>
<version>1.0.12</version>
</dependency>
```

Java SDK支持的最新版本，请在[这儿](https://mvnrepository.com/artifact/com.huawei/openstack4j)查询。

**方式三：**从华为云镜像站下载的方式，如下：

1.  找到本地maven的全局配置文件（settings.xml），该文件通常位于maven安装目录的conf下，例如windows系统中：D:\\maven\\apache-maven-3.3.9\\conf\\settings.xml
2.  在settings.xml找到mirror节点，在mirror节点中增加：

```
<mirror>
    <id>huaweicloud</id>
    <mirrorOf>*,!HuaweiCloudSDK</mirrorOf>
    <url>https://repo.huaweicloud.com/repository/maven/</url>
</mirror>
```

1.  打开Maven工程的pom.xml，在“<dependency\>”节点中加入以下配置：

```
<dependency>
    <groupId>com.huawei</groupId>
    <artifactId>openstack4j</artifactId>
   <version>1.0.12</version>
</dependency>
```

Java SDK支持的最新版本，请在[这儿](https://mvnrepository.com/artifact/com.huawei/openstack4j)查询。

