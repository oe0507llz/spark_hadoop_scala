# spark_hadoop_scala

#### Spark Unable to load native-hadoop library for your platform
https://www.stefaanlippens.net/spark-native-hadoop.html
<br>https://stackoverflow.com/questions/40015416/spark-unable-to-load-native-hadoop-library-for-your-platform
* Download your [hadoop](http://apache-mirror.8birdsvideo.com/hadoop/common/hadoop-3.2.0/hadoop-3.2.0.tar.gz)
* Unpack
* set ```HADOOP_HOME``` to point to that directory
* Add ```export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$HADOOP_HOME/lib/native``` to ```/etc/spark/conf/spark-env.sh ``` and the ```NativeCodeLoader``` warning went away.

