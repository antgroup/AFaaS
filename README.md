# Ant Group Production FaaS Trace Data Releases
This repository provides public releases of Ant Group's production serverless FaaS traces, made accessible to the research and academic community.



## Ant Group Public cold starts

These files include every cold start recorded in our public cloud.

**Duration:** 1-day temporary.

| Metric/link | Description |
|-------------|-------------|
| [20250420.csv](https://mdn.alipayobjects.com/rms_9e20d4/uri/file/as/20250420-upload.csv)          | 1-day temporary         |

**Schema**

This table presents individual cold start events, with each row containing trace information for a cold start event. The details include the timestamp, cluster name, function name, request ID, pod ID, memory cost, total duration, time taken to allocate a pod, time to deploy code, and time to create an instance.

| Name | Description | Unit | Example |
|------|-------------|------|---------|
| day   | day          | date     |         |
|   time   |   timestamp          |   date   |         |
|   clustername   |     cluster name	        |  -    |         |
|   funcname   |     MD5-hashed  function name        |  -    |         |
|   requestid   |   MD5-hashed  traceId |  -    |         |
|   podid   |    MD5-hashed  instanceId         |   -   |         |
|   mem   |       instance memory cost     |  byte    |         |
|   totalcost   |         total time spent on cold start    |    ms  |         |
|   podallocationcost   |   schedule overhead          |   ms   |         |
|   deploycodecost   | time to download, extract, and deploy function code           | ms     |         |
|   createinstancecost   |   Function instance cold start time          |  ms    |         |


