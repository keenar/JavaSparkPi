# JavaSparkPi

./sbin/start-master.sh
$SPARK_HOME/sbin/start-master.sh

./sbin/start-worker.sh <master-spark-URL>

To debug run from terminal:
$SPARK_HOME/bin/spark-submit --class "CalcPi" --master local[4] --conf spark.driver.extraJavaOptions=-agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=7777 {Replace_with_path_to_jar}/JavaSparkPi-1.0-SNAPSHOT.jar
