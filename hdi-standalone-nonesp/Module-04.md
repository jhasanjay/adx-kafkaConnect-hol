

# About

This module covers provisioning an Azure Active Directory (AAD) Service Principal (SPN).  We will grant this SPN, the "ingestor" role in ADX, adn leverage the same to sink to ADX from Kafka  <br>

Navigate to your resource group, and click on "Add" and follow the steps below.<br>

### 1. Search for "Storage Account"
![CreateStorage01](images/01-spn-01.png)
<br>
<hr>
<br>

### 2. Click "create"
![CreateStorage02](images/01-spn-02.png)
<br>
<hr>
<br>

### 3. Enter details, be sure to select the right resource group and region
![CreateStorage03](images/01-spn-03.png)
<br>
<hr>
<br>


### 4. Select Locally Redundant Storage
![CreateStorage05](images/01-spn-05.png)
<br>
<hr>
<br>

### 5. In the advanced tab, leave defaults
![CreateStorage06](images/01-spn-06.png)
<br>
<hr>
<br>

### 6. Validate and click "create"
![CreateStorage07](images/01-spn-07.png)
<br>
<hr>
<br>

### 7. Once the service is provisioned, click on it in your resource group, we will create containers
![CreateStorage08](images/01-spn-08.png)
<br>
<hr>
<br>

### 8. Click on "Containers"
![CreateStorage09](images/01-spn-09.png)
<br>
<hr>
<br>

### 9. Click on "+Container"
![CreateStorage10](images/03-storage-10.png)
<br>
<hr>
<br>

This concludes the module.<br>
[Return to the menu](https://github.com/anagha-microsoft/adx-kafkaConnect-hol/tree/master/hdi-standalone-nonesp#lets-get-started)
