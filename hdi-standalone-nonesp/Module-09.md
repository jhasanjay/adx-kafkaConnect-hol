

# About

This module covers downloading and configuring KafkaConnect for ADX and launching the service. 
<br>

### 1. SSH to the edge node ands switch to root

![CreateHDI01](images/02-hdi-41.png)
<br>
<hr>
<br>

![CreateHDI01](images/02-hdi-42.png)
<br>
<hr>
<br>

### 2. Install tree

```
apt-get install -y tree
```

![CreateHDI01](images/06-kck-01.png)
<br>
<hr>
<br>

### 3. Create directory path for KafkaConnect jar download

```
 mkdir -p opt/kafka-connect-kusto
```

```
 tree opt
```

![CreateHDI01](images/06-kck-02.png)
<br>
<hr>
<br>

### 4. Change to the directory created and download the jar

```
cd opt/kafka-connect-kusto
```

```
wget "https://github.com/Azure/kafka-sink-azure-kusto/releases/download/v0.3.2/kafka-sink-azure-kusto-0.3.2-jar-with-dependencies.jar"
```


![CreateHDI01](images/06-kck-02.png)
<br>
<hr>
<br>


This concludes the module.<br>
[Return to the menu](https://github.com/anagha-microsoft/adx-kafkaConnect-hol/tree/master/hdi-standalone-nonesp#lets-get-started)
