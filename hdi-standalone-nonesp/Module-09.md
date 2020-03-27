

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


![CreateHDI01](images/06-kck-03.png)
<br>
<hr>
<br>

### 5. Rename the jar to have the prefix of 'kafka-connect'.  This is important because the default scripts that execute KafkaConnect search for jars starting with this name.

```
ls -al
```

```
mv kafka-sink-azure-kusto-0.3.2-jar-with-dependencies.jar kafka-connect-kusto-sink-0.3.2-uber.jar
```

![CreateHDI01](images/06-kck-04a.png)
<br>
<hr>
<br>

![CreateHDI01](images/06-kck-04b.png)
<br>
<hr>
<br>

### 6. Make the jar executable

```
chmod +x kafka-connect-kusto-sink-0.3.2-uber.jar 
```

![CreateHDI01](images/06-kck-05a.png)
<br>
<hr>
<br>

### 7. Copy the jar to the two directory paths (till we can reconcile to one path)

1.  Copy to /usr/hdp/current/kafka-broker/libs/

```
cp kafka-connect-kusto-sink-0.3.2-uber.jar /usr/hdp/current/kafka-broker/libs/
```

```
ls -al /usr/hdp/current/kafka-broker/libs/ | grep kusto
```

![CreateHDI01](images/06-kck-06a.png)
<br>
<hr>
<br>

2.   Copy to /usr/share/java/

```
cp kafka-connect-kusto-sink-0.3.2-uber.jar /usr/share/java/
```

```
ls -al /usr/share/java/ | grep kusto
```

![CreateHDI01](images/06-kck-06b.png)
<br>
<hr>
<br>


This concludes the module.<br>
[Return to the menu](https://github.com/anagha-microsoft/adx-kafkaConnect-hol/tree/master/hdi-standalone-nonesp#lets-get-started)
