# Eureka Server Sample

Start 2 instances of this application.

java -jar target/eureka-0.0.1-SNAPSHOT.jar --spring.profiles.active=peer
AND
java -jar target/eureka-0.0.1-SNAPSHOT.jar --spring.profiles.active=other


Give it a few minutes for eureka to do its thing then visit the following URL's
and note that in the status and info enpoint pages that the  ${management.contextPath} property has not been resolved.

http://127.0.0.1:8762/eureka/apps
http://127.0.0.1:8761/eureka/apps

```
This XML file does not appear to have any style information associated with it. The document tree is shown below.
<applications>
<versions__delta>1</versions__delta>
<apps__hashcode>UP_2_</apps__hashcode>
<application>
<name>EUREKA</name>
<instance>
<hostName>127.0.1.1</hostName>
<app>EUREKA</app>
<ipAddr>10.130.4.70</ipAddr>
<status>UP</status>
<overriddenstatus>UNKNOWN</overriddenstatus>
<port enabled="true">8761</port>
<securePort enabled="false">443</securePort>
<countryId>1</countryId>
<dataCenterInfo class="com.netflix.appinfo.InstanceInfo$DefaultDataCenterInfo">
<name>MyOwn</name>
</dataCenterInfo>
<leaseInfo>
<renewalIntervalInSecs>30</renewalIntervalInSecs>
<durationInSecs>90</durationInSecs>
<registrationTimestamp>1424698426619</registrationTimestamp>
<lastRenewalTimestamp>1424698606649</lastRenewalTimestamp>
<evictionTimestamp>0</evictionTimestamp>
<serviceUpTimestamp>1424698396573</serviceUpTimestamp>
</leaseInfo>
<metadata class="java.util.Collections$EmptyMap"/>
<homePageUrl>http://127.0.1.1:8761/</homePageUrl>
<statusPageUrl>
http://127.0.1.1:8761${management.contextPath}/info
</statusPageUrl>
<healthCheckUrl>
http://127.0.1.1:8761${management.contextPath}/health
</healthCheckUrl>
<vipAddress>eureka</vipAddress>
<isCoordinatingDiscoveryServer>false</isCoordinatingDiscoveryServer>
<lastUpdatedTimestamp>1424698426619</lastUpdatedTimestamp>
<lastDirtyTimestamp>1424698406186</lastDirtyTimestamp>
<actionType>ADDED</actionType>
</instance>
<instance>
<hostName>127.0.0.1</hostName>
<app>EUREKA</app>
<ipAddr>10.130.4.70</ipAddr>
<status>UP</status>
<overriddenstatus>UNKNOWN</overriddenstatus>
<port enabled="true">8762</port>
<securePort enabled="false">443</securePort>
<countryId>1</countryId>
<dataCenterInfo class="com.netflix.appinfo.InstanceInfo$DefaultDataCenterInfo">
<name>MyOwn</name>
</dataCenterInfo>
<leaseInfo>
<renewalIntervalInSecs>30</renewalIntervalInSecs>
<durationInSecs>90</durationInSecs>
<registrationTimestamp>1424698450746</registrationTimestamp>
<lastRenewalTimestamp>1424698601028</lastRenewalTimestamp>
<evictionTimestamp>0</evictionTimestamp>
<serviceUpTimestamp>1424698421140</serviceUpTimestamp>
</leaseInfo>
<metadata class="java.util.Collections$EmptyMap"/>
<homePageUrl>http://127.0.0.1:8762/</homePageUrl>
<statusPageUrl>
http://127.0.0.1:8762${management.contextPath}/info
</statusPageUrl>
<healthCheckUrl>
http://127.0.0.1:8762${management.contextPath}/health
</healthCheckUrl>
<vipAddress>eureka</vipAddress>
<isCoordinatingDiscoveryServer>true</isCoordinatingDiscoveryServer>
<lastUpdatedTimestamp>1424698450746</lastUpdatedTimestamp>
<lastDirtyTimestamp>1424698430488</lastDirtyTimestamp>
<actionType>ADDED</actionType>
</instance>
</application>
</applications>
```
