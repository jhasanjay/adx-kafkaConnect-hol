

# About

This module covers provisioning an Azure Active Directory (AAD) Service Principal (SPN).  We will grant this SPN, the "ingestor" role in ADX, adn leverage the same to sink to ADX from Kafka  <br>

Navigate to portal.azure.com on your browser and follow the steps below:<br>

### 1. Click on Azure Active Directory
![CreateStorage01](images/01-spn-01.png)
<br>
<hr>
<br>

### 2. Click on App Registrations
![CreateStorage02](images/01-spn-02.png)
<br>
<hr>
<br>

### 3. Click on New Registration
![CreateStorage03](images/01-spn-03.png)
<br>
<hr>
<br>


### 4. Select Locally Redundant Storage
![CreateStorage05](images/01-spn-04.png)
<br>
<hr>
<br>

### 5. In the advanced tab, leave defaults
![CreateStorage06](images/01-spn-05.png)
<br>
<hr>
<br>

### 6. Validate and click "create"
![CreateStorage07](images/01-spn-06.png)
<br>
<hr>
<br>

### 7. Once the service is provisioned, click on it in your resource group, we will create containers
![CreateStorage08](images/01-spn-07.png)
<br>
<hr>
<br>

### 8. Click on "Containers"
![CreateStorage09](images/01-spn-08.png)
<br>
<hr>
<br>

### 9. Click on "Containers"
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
