> step 1: install hadoop 3.0

> step 2: hdfs erasurecode -listPolicies
```
RS-DEFAULT-3-2-64k, RS-DEFAULT-6-3-64k, RS-LEGACY-6-3-64k
```
> setp 3: hdfs dfs -mkdir /test-RS-DEFAULT-3-2-64k

> step 4: hdfs dfs -put package/data.info /test-RS-DEFAULT-3-2-64k/

> step 5: hdfs dfs -du -h /test*
```
50 M  150 M   /test/data.info
50 M  83.4 M  /test-RS-DEFAULT-3-2-64k/data.info
```


