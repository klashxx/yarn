
# yarn.py

```text
$ ./yarn.py  -h
usage: yarn.py [-h]
               [--status {ALL,NEW,NEW_SAVING,SUBMITTED,ACCEPTED,RUNNING,FINISHED,FAILED,KILLED}]
               [--head HEAD] [--asc]

yarn extended

optional arguments:
  -h, --help            show this help message and exit
  --status {ALL,NEW,NEW_SAVING,SUBMITTED,ACCEPTED,RUNNING,FINISHED,FAILED,KILLED}
                        app status [default ALL]
  --head HEAD           first n rows [default 1000]
  --asc                 start time in ASC order [Default False]
```

```text
$ ./yarn.py --status RUNNING --status KILLED --head 20
---------------------------------------------------------------------------------------------------------------------------------------------
| ID                             | Name                      | State      | User       | Type       | Start               | Duration        |
---------------------------------------------------------------------------------------------------------------------------------------------
| application_1646273095080_0233 | TEST_STREAM_JOB_01        | RUNNING    | tstuser    | SPARK      | 2022-03-08 12:59:06 | 1 day, 0:56:00  |
| application_1646273095080_0231 | TEST_STREAM_JOB_02        | RUNNING    | tstuser    | SPARK      | 2022-03-08 11:54:19 | 1 day, 2:00:45  |
| application_1642565008363_0351 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 15:06:44 | 0:45:00         |
| application_1642565008363_0350 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 14:06:43 | 0:45:01         |
| application_1642565008363_0347 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 13:06:43 | 0:45:02         |
| application_1642565008363_0346 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 12:06:43 | 0:45:01         |
| application_1642565008363_0345 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 11:06:43 | 0:45:02         |
| application_1642565008363_0344 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 10:06:43 | 0:45:01         |
| application_1642565008363_0343 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 09:06:43 | 0:45:01         |
| application_1642565008363_0340 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 08:06:43 | 0:45:01         |
| application_1642565008363_0339 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 07:06:43 | 0:45:01         |
| application_1642565008363_0338 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 06:06:42 | 0:45:01         |
| application_1642565008363_0337 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 05:06:42 | 0:45:01         |
| application_1642565008363_0336 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 04:06:42 | 0:45:02         |
| application_1642565008363_0335 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 03:06:42 | 0:45:01         |
| application_1642565008363_0334 | CMYarnUsageAggregation    | KILLED     | mnguser    | MAPREDUCE  | 2022-01-27 02:06:42 | 0:45:01         |
---------------------------------------------------------------------------------------------------------------------------------------------
```
