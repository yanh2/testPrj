# testPrj
## Prerequistic
### hostname 
* master is hadoop master
* example
```
sudo -i
echo "111.111.111.111 (하둡 아이피)master" >> /etc/hosts
```

### keyfile
* keyfile name : mykey.pem
```
$ ls
do.sh  hive_empdept.sh  mykey.pem
```

## install
```
git clone http://github.com/
cd testPrj/
scp ~/mykey.pem ./
. do.sh
```

## Result
```
Time taken: 10.83 seconds, Fetched: 3 row(s)
Query ID = hadoop_20200107050323_39d3663c-b943-4037-98fe-042f32f4a785
Total jobs = 1
Launching Job 1 out of 1
Status: Running (Executing on YARN cluster with App id application_1578362765879_0007)

Map 1: 0(+1)/1  Reducer 2: 0/1  Reducer 3: 0/1
Map 1: 1/1      Reducer 2: 0/1  Reducer 3: 0/1
Map 1: 1/1      Reducer 2: 1/1  Reducer 3: 0(+1)/1
Map 1: 1/1      Reducer 2: 1/1  Reducer 3: 1/1
OK
20      2518.75
10      2916.6666666666665
Time taken: 1.167 seconds, Fetched: 2 row(s)
OK
dept
emp
Time taken: 0.028 seconds, Fetched: 2 row(s)
```

## Copy Right
2020.01 hyanj14@gmail.com
