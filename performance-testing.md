## Performance Testing

````
Channel_1: Master_Bangalore (Starting time: 11:17 AM)
Channel_2: Master_Munich (Starting time: 11:52 AM)
Replica
````

First started Master_Bangalore \
Then started Master_Munich


### Test 1: Checked at 12:00 PM 🕧 (`seconds_behind_master`)
**Master_Bangalore = 0** (Up-to-date) 
**Master_Munich = 234** (3.9 minutes delay) 

###### Records:
In Master_Munich: 275914 \
In Replica:       152192

##### *Observation*: After 8 minutes of execution in Master_Munich, replica was 3.9 minutes behind


### Test 2: Checked at 12:06 PM 🕧 (`seconds_behind_master`)
**Master_Bangalore = 0**\
**Master_Munich = 384** ( 6.4 minutes) 

##### *Observation*: After 14 minutes of execution in Master_Munich, replica was 6.4 minutes behind



### Test 3: Checked at 12:30 PM 🕧 (`seconds_behind_master`)
**Master_Bangalore = 0** (Up-to-date) \
**Master_Munich = 969** ( 16 minutes delay) 

###### Records:
In Master_Munich: 1343678 \
In Replica:       780700

##### *Observation*: After 38 minutes of execution in Master_Munich, replica was 16 minutes behind



### Test 4: Stopped Master_Munich process at 12:35 PM 🕧 (`seconds_behind_master`)
**Master_Bangalore = 0**\ (Up-to-date)
**Master_Munich = 1091** ( 18.1 minutes delay) 

##### *Observation*: After 43 minutes of execution in Master_Munich, replica was 18.1 minutes behind

## Conclusion

##### It took 27 minutes to cover the gap after stopping the process and at 1:02 PM 🕧, both master and replica were at the same state of **

###### Records:
In Master_Munich: 1533649 \
In Replica:       1533649 \
\


````
Few unique point:

1: @12:17 PM Stopped Master_Bangalore process, again started 12:31 PM and check later 12:40 PM \
but still there was **no lag** in Master_Bangalore

2: Started Master_Munich first and later started Master_Bangalore but still Master_Munich was behind.

````





