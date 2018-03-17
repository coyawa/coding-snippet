```sh
Tips-Hadoop



Resource Manager: http://localhost:50070
JobTracker: http://localhost:8088
Specific Node Information: http://localhost:8042
通过他们可以访问 HDFS filesystem, 也可以取得结果输出文件.

http://blog.csdn.net/yechaodechuntian/article/details/44312343

http://www.voidcn.com/blog/epeaktop/article/p-6003117.html

6.可视化查看
* 通过web接口查看
* Cluster Status http://localhost:8088
* HDFS status http://localhost:50070
* secondaryNamenode http://localhost:50090

.profile
alias hstart="/usr/local/Cellar/hadoop/2.7.3/sbin/start-dfs.sh;/usr/local/Cellar/hadoop/2.7.3/sbin/start-yarn.sh"
alias hstop="/usr/local/Cellar/hadoop/2.7.3/sbin/stop-yarn.sh;/usr/local/Cellar/hadoop/2.7.3/sbin/stop-dfs.sh"

启动与关闭
启动HADOOP
1.         进入HADOOP_HOME目录。
2.         执行sh sbin/start-all.sh
关闭HADOOP
1.         进入HADOOP_HOME目录。
2.         执行sh sbin/stop-all.sh

/usr/local/Cellar/hadoop/2.7.3/sbin/start-dfs.sh
/usr/local/Cellar/hadoop/2.7.3/sbin/stop-yarn.sh

Hadoop_ev

export HADOOP_CLASSPATH=${JAVA_HOME}/lib/tools.jar


4.rm
hadoop fs -rm < hdfs file > ...
hadoop fs -rm -r < hdfs dir>...
每次可以删除多个文件或目录

5.mkdir
hadoop fs -mkdir < hdfs path>
只能一级一级的建目录，父目录不存在的话使用这个命令会报错
hadoop fs -mkdir -p < hdfs path> ha
所创建的目录如果父目录不存在就创建该父目录

2.put
hadoop fs -put < local file > < hdfs file >
hdfs file的父目录一定要存在，否则命令不会执行
hadoop fs -put  < local file or dir >...< hdfs dir >
hdfs dir 一定要存在，否则命令不会执行

编译java to java and class
1. hadoop com.sun.tools.javac.Main P1.java
2. jar cf P1.jar P1*.class

6. 查看结果文件
hadoop fs -cat /user/Coyawa/output/1/part-r-00000


需要注意的是，指定输入输出文件时，需要指定hdfs的URI，比如输入目录是hdfs://hadoop-test/tmp/input，输出目录是hdfs://hadoop-test/tmp/output，其中，“hdfs://hadoop-test”是由Hadoop配置文件core-site.xml中参数fs.default.name指定的，具体替换成你的配置即可。

```