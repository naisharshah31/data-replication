  ## Long Running Test for Multi Source Data Replication

| Friday 2022-04-29 6:35 PM | Naishar | Rohan | PI |
| ------------------------- | ------- | ----- | -- |
|  | 0 | 0 | 0 |


| Monday 2022-05-02 10:15 AM | Naishar | Rohan | PI |
| ------------------------- | ------- | ----- | -- |
|  | 226351 | 227914 | 454265 | 


**OBSERVATION:** Test ran for almost 64 hours and there was **no lag**. Every second both the masters were writting to raspberry pi for almost \
straight 64 hours.


## Interval Test for Multi Source Data Replication

#### 5 minutes 

|     5 minutes interval   |      |     |    |
| -------------------------| ---- | --- | -- |
| 12:35 | Naishar | Rohan | PI |
| 12:40 | 298 | 299 | 597 |

|     5 minutes interval   |      |     |    |
| -------------------------| ---- | --- | -- |
| 12:45 | Naishar | Rohan | PI |
| 12:50 | 297 | 297 | 594 |

|     5 minutes interval   |      |     |    |
| -------------------------| ---- | --- | -- |
| 12:55 | Naishar | Rohan | PI |
| 13:00 | 297 | 298 | 595 |


##### 10 minutes

|     10 minutes interval   |      |     |    |
| -------------------------| ---- | --- | -- |
| 13:50 | Naishar | Rohan | PI |
| 14:00 | 593 | 596 | 1189 |

|     10 minutes interval   |      |     |    |
| -------------------------| ---- | --- | -- |
| 14:05 | Naishar | Rohan | PI |
| 14:15 | 593 | 595 | 1188 |

|     10 minutes interval   |      |     |    |
| -------------------------| ---- | --- | -- |
| 14:20 | Naishar | Rohan | PI |
| 14:30 | 594 | 596 | 1190 |


#### 15 mintues

|     15 minutes interval   |      |     |    |
| -------------------------| ---- | --- | -- |
| 14:40 | Naishar | Rohan | PI |
| 14:55 | 891 | 894 | 1785 |


|     15 minutes interval   |      |     |    |
| -------------------------| ---- | --- | -- |
| 15:00 | Naishar | Rohan | PI |
| 15:15 | 890 | 894 | 1784 |


|     15 minutes interval   |      |     |    |
| -------------------------| ---- | --- | -- |
| 15:20 | Naishar | Rohan | PI |
| 15:35 | 890 | 893 | 1783 |


Observation: Both masters were writting in the database every second and it will be replicated to Raspberry Pi				
Executed this test for intervals of 5 minutes, 10 minutes and 15 minutes and there was no lag.				
