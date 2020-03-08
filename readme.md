
## Question 1
How did changing values on the SparkSession property parameters affect the throughput and latency of the data?
```
It changes the task time under the Executors tab in the SPARK UI
```

## Question 2
What were the 2-3 most efficient SparkSession property key/value pairs? Through testing multiple variations on values, how can you tell these were the most optimal?
```
spark.default.parallelism - increasing this improves throughput in general, provided there is sufficient memory
spark.sql.shuffle.partitions - tweak this based on data size
```