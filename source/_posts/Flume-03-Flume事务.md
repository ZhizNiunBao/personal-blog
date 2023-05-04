---
title: Flume-03-Flume事务
typora-copy-images-to: ./Flume-03-Flume事务
typora-root-url: ./Flume-03-Flume事务
date: 2023-03-14 21:05:55
tags:
categories:
---

# Flume-03-Flume事务

<!--more-->

  ![image-20230314222701993](/image-20230314222701993.png)

![image-20230314222711779](/image-20230314222711779.png)

![image-20230314222723229](/image-20230314222723229.png)











 -Dlog.file=/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/log/flink-root-sql-client-hadoop102.log -Dlog4j.configuration=file:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/conf/log4j-cli.properties -Dlog4j.configurationFile=file:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/conf/log4j-cli.properties -Dlogback.configurationFile=file:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/conf/logback.xml -classpath /Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/lib/flink-csv-1.14-SNAPSHOT.jar:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/lib/flink-json-1.14-SNAPSHOT.jar:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/lib/flink-shaded-zookeeper-3.4.14.jar:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/lib/flink-table_2.11-1.14-SNAPSHOT.jar:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/lib/log4j-1.2-api-2.17.1.jar:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/lib/log4j-api-2.17.1.jar:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/lib/log4j-core-2.17.1.jar:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/lib/log4j-slf4j-impl-2.17.1.jar:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/lib/flink-dist_2.11-1.14-SNAPSHOT.jar:/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/opt/flink-python_2.11-1.14-SNAPSHOT.jar::/Users/huangxiaoli/IdeaProjects/flink-1.14/flink-dist/target/flink-1.14-SNAPSHOT-bin/flink-1.14-SNAPSHOT/opt/flink-sql-client_2.11-1.14-SNAPSHOT.jar org.apache.flink.table.client.SqlClient --jar /opt/module/flink-1.14.6/opt/flink-sql-client_2.12-1.14.6.jar





CREATE TABLE test1 (
  id INT
) WITH (
   'connector' = 'datagen'

);
