[zhou@ip-172-31-38-40 ~]$ time hadoop jar /opt/cloudera/parcels/CDH-5.11.0-1.cdh5.11.0.p0.34/jars/hadoop-examples.jar teragen -Dmapred.map.tasks=8 -Dmapreduce.map.memory.mb=512 -Ddfs.block.size=16777216 65536000  /user/zhou/tgen5
17/05/12 04:34:48 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-37-46.us-west-2.compute.internal/172.31.37.46:8032
17/05/12 04:34:49 INFO terasort.TeraGen: Generating 65536000 using 8
17/05/12 04:34:49 INFO mapreduce.JobSubmitter: number of splits:8
17/05/12 04:34:49 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
17/05/12 04:34:49 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/05/12 04:34:49 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494562242244_0002
17/05/12 04:34:49 INFO impl.YarnClientImpl: Submitted application application_1494562242244_0002
17/05/12 04:34:49 INFO mapreduce.Job: The url to track the job: http://ip-172-31-37-46.us-west-2.compute.internal:8088/proxy/application_1494562242244_0002/
17/05/12 04:34:49 INFO mapreduce.Job: Running job: job_1494562242244_0002
17/05/12 04:34:57 INFO mapreduce.Job: Job job_1494562242244_0002 running in uber mode : false
17/05/12 04:34:57 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 04:35:16 INFO mapreduce.Job:  map 9% reduce 0%
17/05/12 04:35:18 INFO mapreduce.Job:  map 15% reduce 0%
17/05/12 04:35:19 INFO mapreduce.Job:  map 25% reduce 0%
17/05/12 04:35:22 INFO mapreduce.Job:  map 26% reduce 0%
17/05/12 04:35:24 INFO mapreduce.Job:  map 28% reduce 0%
17/05/12 04:35:25 INFO mapreduce.Job:  map 30% reduce 0%
17/05/12 04:35:28 INFO mapreduce.Job:  map 32% reduce 0%
17/05/12 04:35:31 INFO mapreduce.Job:  map 36% reduce 0%
17/05/12 04:35:32 INFO mapreduce.Job:  map 37% reduce 0%
17/05/12 04:35:34 INFO mapreduce.Job:  map 38% reduce 0%
17/05/12 04:35:37 INFO mapreduce.Job:  map 44% reduce 0%
17/05/12 04:35:38 INFO mapreduce.Job:  map 45% reduce 0%
17/05/12 04:35:40 INFO mapreduce.Job:  map 47% reduce 0%
17/05/12 04:35:43 INFO mapreduce.Job:  map 52% reduce 0%
17/05/12 04:35:46 INFO mapreduce.Job:  map 53% reduce 0%
17/05/12 04:35:48 INFO mapreduce.Job:  map 55% reduce 0%
17/05/12 04:35:49 INFO mapreduce.Job:  map 58% reduce 0%
17/05/12 04:35:52 INFO mapreduce.Job:  map 60% reduce 0%
17/05/12 04:35:54 INFO mapreduce.Job:  map 62% reduce 0%
17/05/12 04:35:56 INFO mapreduce.Job:  map 65% reduce 0%
17/05/12 04:35:58 INFO mapreduce.Job:  map 66% reduce 0%
17/05/12 04:36:01 INFO mapreduce.Job:  map 69% reduce 0%
17/05/12 04:36:02 INFO mapreduce.Job:  map 70% reduce 0%
17/05/12 04:36:04 INFO mapreduce.Job:  map 72% reduce 0%
17/05/12 04:36:07 INFO mapreduce.Job:  map 76% reduce 0%
17/05/12 04:36:10 INFO mapreduce.Job:  map 78% reduce 0%
17/05/12 04:36:12 INFO mapreduce.Job:  map 79% reduce 0%
17/05/12 04:36:13 INFO mapreduce.Job:  map 83% reduce 0%
17/05/12 04:36:15 INFO mapreduce.Job:  map 84% reduce 0%
17/05/12 04:36:19 INFO mapreduce.Job:  map 86% reduce 0%
17/05/12 04:36:20 INFO mapreduce.Job:  map 90% reduce 0%
17/05/12 04:36:25 INFO mapreduce.Job:  map 92% reduce 0%
17/05/12 04:36:26 INFO mapreduce.Job:  map 96% reduce 0%
17/05/12 04:36:29 INFO mapreduce.Job:  map 98% reduce 0%
17/05/12 04:36:30 INFO mapreduce.Job:  map 100% reduce 0%
17/05/12 04:36:30 INFO mapreduce.Job: Job job_1494562242244_0002 completed successfully
17/05/12 04:36:30 INFO mapreduce.Job: Counters: 33
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=1020864
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=682
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=32
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters 
                Launched map tasks=8
                Other local map tasks=8
                Total time spent by all maps in occupied slots (ms)=688384
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=688384
                Total vcore-milliseconds taken by all map tasks=688384
                Total megabyte-milliseconds taken by all map tasks=704905216
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=682
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=2171
                CPU time spent (ms)=139320
                Physical memory (bytes) snapshot=1476825088
                Virtual memory (bytes) snapshot=8982827008
                Total committed heap usage (bytes)=1882193920
                Peak Map Physical memory (bytes)=249737216
                Peak Map Virtual memory (bytes)=1129971712
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters 
                Bytes Read=0
        File Output Format Counters 
                Bytes Written=6553600000

real    1m45.031s
user    0m5.850s
sys     0m0.712s
[zhou@ip-172-31-38-40 ~]$ hdfs dfs -ls /user/zhou/tgen
ls: `/user/zhou/tgen': No such file or directory
[zhou@ip-172-31-38-40 ~]$ time hadoop jar /opt/cloudera/parcels/CDH-5.11.0-1.cdh5.11.0.p0.34/jars/hadoop-examples.jar teragen -Dmapred.map.tasks=8 -Dmapreduce.map.memory.mb=512 -Ddfs.block.size=16777216 65536000  /user/zhou/tgen5^C
[zhou@ip-172-31-38-40 ~]$ hdfs dfs -ls /user/zhou/tgen5
Found 9 items
-rw-r--r--   3 zhou beijing          0 2017-05-12 04:36 /user/zhou/tgen5/_SUCCESS
-rw-r--r--   3 zhou beijing  819200000 2017-05-12 04:36 /user/zhou/tgen5/part-m-00000
-rw-r--r--   3 zhou beijing  819200000 2017-05-12 04:36 /user/zhou/tgen5/part-m-00001
-rw-r--r--   3 zhou beijing  819200000 2017-05-12 04:36 /user/zhou/tgen5/part-m-00002
-rw-r--r--   3 zhou beijing  819200000 2017-05-12 04:36 /user/zhou/tgen5/part-m-00003
-rw-r--r--   3 zhou beijing  819200000 2017-05-12 04:36 /user/zhou/tgen5/part-m-00004
-rw-r--r--   3 zhou beijing  819200000 2017-05-12 04:36 /user/zhou/tgen5/part-m-00005
-rw-r--r--   3 zhou beijing  819200000 2017-05-12 04:36 /user/zhou/tgen5/part-m-00006
-rw-r--r--   3 zhou beijing  819200000 2017-05-12 04:36 /user/zhou/tgen5/part-m-00007
[zhou@ip-172-31-38-40 ~]$ 

another  test:
[zhou@ip-172-31-38-40 ~]$ time hadoop jar /opt/cloudera/parcels/CDH-5.11.0-1.cdh5.11.0.p0.34/jars/hadoop-examples.jar teragen -Dmapred.map.tasks=6 -Dmapreduce.map.memory.mb=1024 -Ddfs.block.size=67108864 65536000  /user/zhou/tgen5
java.io.IOException: Output directory /user/zhou/tgen5 already exists.
        at org.apache.hadoop.examples.terasort.TeraGen.run(TeraGen.java:293)
        at org.apache.hadoop.util.ToolRunner.run(ToolRunner.java:70)
        at org.apache.hadoop.examples.terasort.TeraGen.main(TeraGen.java:309)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.util.ProgramDriver$ProgramDescription.invoke(ProgramDriver.java:71)
        at org.apache.hadoop.util.ProgramDriver.run(ProgramDriver.java:144)
        at org.apache.hadoop.examples.ExampleDriver.main(ExampleDriver.java:74)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.util.RunJar.run(RunJar.java:221)
        at org.apache.hadoop.util.RunJar.main(RunJar.java:136)

real    0m2.821s
user    0m3.215s
sys     0m0.473s
[zhou@ip-172-31-38-40 ~]$ time hadoop jar /opt/cloudera/parcels/CDH-5.11.0-1.cdh5.11.0.p0.34/jars/hadoop-examples.jar teragen -Dmapred.map.tasks=6 -Dmapreduce.map.memory.mb=1024 -Ddfs.block.size=67108864 65536000  /user/zhou/tgen
17/05/12 04:52:07 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-37-46.us-west-2.compute.internal/172.31.37.46:8032
17/05/12 04:52:08 INFO terasort.TeraGen: Generating 65536000 using 6
17/05/12 04:52:08 INFO mapreduce.JobSubmitter: number of splits:6
17/05/12 04:52:08 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
17/05/12 04:52:08 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/05/12 04:52:08 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494562242244_0003
17/05/12 04:52:08 INFO impl.YarnClientImpl: Submitted application application_1494562242244_0003
17/05/12 04:52:08 INFO mapreduce.Job: The url to track the job: http://ip-172-31-37-46.us-west-2.compute.internal:8088/proxy/application_1494562242244_0003/
17/05/12 04:52:08 INFO mapreduce.Job: Running job: job_1494562242244_0003
17/05/12 04:52:16 INFO mapreduce.Job: Job job_1494562242244_0003 running in uber mode : false
17/05/12 04:52:16 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 04:52:35 INFO mapreduce.Job:  map 8% reduce 0%
17/05/12 04:52:36 INFO mapreduce.Job:  map 23% reduce 0%
17/05/12 04:52:41 INFO mapreduce.Job:  map 26% reduce 0%
17/05/12 04:52:42 INFO mapreduce.Job:  map 29% reduce 0%
17/05/12 04:52:48 INFO mapreduce.Job:  map 36% reduce 0%
17/05/12 04:52:54 INFO mapreduce.Job:  map 43% reduce 0%
17/05/12 04:53:00 INFO mapreduce.Job:  map 51% reduce 0%
17/05/12 04:53:05 INFO mapreduce.Job:  map 53% reduce 0%
17/05/12 04:53:06 INFO mapreduce.Job:  map 58% reduce 0%
17/05/12 04:53:11 INFO mapreduce.Job:  map 61% reduce 0%
17/05/12 04:53:12 INFO mapreduce.Job:  map 66% reduce 0%
17/05/12 04:53:17 INFO mapreduce.Job:  map 68% reduce 0%
17/05/12 04:53:18 INFO mapreduce.Job:  map 73% reduce 0%
17/05/12 04:53:23 INFO mapreduce.Job:  map 75% reduce 0%
17/05/12 04:53:24 INFO mapreduce.Job:  map 80% reduce 0%
17/05/12 04:53:30 INFO mapreduce.Job:  map 83% reduce 0%
17/05/12 04:53:31 INFO mapreduce.Job:  map 86% reduce 0%
17/05/12 04:53:36 INFO mapreduce.Job:  map 93% reduce 0%
17/05/12 04:53:40 INFO mapreduce.Job:  map 94% reduce 0%
17/05/12 04:53:41 INFO mapreduce.Job:  map 95% reduce 0%
17/05/12 04:53:42 INFO mapreduce.Job:  map 100% reduce 0%
17/05/12 04:53:43 INFO mapreduce.Job: Job job_1494562242244_0003 completed successfully
17/05/12 04:53:43 INFO mapreduce.Job: Counters: 33
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=765648
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=511
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=24
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=12
        Job Counters 
                Launched map tasks=6
                Other local map tasks=6
                Total time spent by all maps in occupied slots (ms)=494913
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=494913
                Total vcore-milliseconds taken by all map tasks=494913
                Total megabyte-milliseconds taken by all map tasks=506790912
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=511
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1233
                CPU time spent (ms)=125060
                Physical memory (bytes) snapshot=1993412608
                Virtual memory (bytes) snapshot=9444569088
                Total committed heap usage (bytes)=2001207296
                Peak Map Physical memory (bytes)=386727936
                Peak Map Virtual memory (bytes)=1577992192
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters 
                Bytes Read=0
        File Output Format Counters 
                Bytes Written=6553600000

real    1m38.760s
user    0m5.757s
sys     0m0.728s
[zhou@ip-172-31-38-40 ~]$ hdfs dfs -ls /user/zhou/tgen
Found 7 items
-rw-r--r--   3 zhou beijing          0 2017-05-12 04:53 /user/zhou/tgen/_SUCCESS
-rw-r--r--   3 zhou beijing 1092266700 2017-05-12 04:53 /user/zhou/tgen/part-m-00000
-rw-r--r--   3 zhou beijing 1092266700 2017-05-12 04:53 /user/zhou/tgen/part-m-00001
-rw-r--r--   3 zhou beijing 1092266600 2017-05-12 04:53 /user/zhou/tgen/part-m-00002
-rw-r--r--   3 zhou beijing 1092266700 2017-05-12 04:53 /user/zhou/tgen/part-m-00003
-rw-r--r--   3 zhou beijing 1092266700 2017-05-12 04:53 /user/zhou/tgen/part-m-00004
-rw-r--r--   3 zhou beijing 1092266600 2017-05-12 04:53 /user/zhou/tgen/part-m-00005
[zhou@ip-172-31-38-40 ~]$ 
