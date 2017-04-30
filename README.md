DropWizard Example
======

##Shipping Calculation Service using Netuitive Metrics

Down load the repository and update the API Key in shippingservice.yaml with your Custom Integration API Key from Netuitive.

Build the project using gradle

```
C:\ShippingService> gradlew clean build packageJar
```
or
```
$ ./gradlew clean build packageJar
```

Next run the application using the following command
```
 java -jar ./build/libs/dropwizard_shipping_service_with_metrics-1.0-SNAPSHOT-standalone.jar server shippingservice.yaml
```

Your service should now be running on [localhost:8080](http://localhost:8080)

Try the following interactions

[http://localhost:8080/calculate?weight=1](http://localhost:8080/calculate?weight=1)

[http://localhost:8080/calculate?weight=2](http://localhost:8080/calculate?weight=2)

[http://localhost:8080/calculate?weight=10](http://localhost:8080/calculate?weight=10)

