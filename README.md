# proiect-sosm

My name is Ionescu-Tautu Mihai-Andrei and for my SOSM project I developed an e-store app consisting of the following: 
* a rest-based web-service for fetching the list of available products (catalog-service)
* a webserver for displaying/ordering products (catalog-webapp)
* a mobile app that uses both the web-service and the server (Catalog)

In terms of databases, I used a local mysql instance that is mirrored on the android side for app caching/offline-availability. The web-service and server were developed using Java technologies (jaxrs, jetty, jsp etc) and the mobile app was done using the Android SDK.

For running the project:
1. import the catalog.sql file on a local mysql server instance.
2. deploy the catalog-webapp.war and catalog-service WARs on a local Tomcat/Jetty/Glassish instance.
3. Before starting the android app, update the SERVICEURL string in [MainActivity.java](https://github.com/itma96/proiect-sosm/blob/master/Catalog/app/src/main/java/com/example/andrei/catalog/MainActivity.java) and the WEBAPPURL string in [CustomAdapter.java](https://github.com/itma96/proiect-sosm/blob/master/Catalog/app/src/main/java/com/example/andrei/catalog/CustomAdapter.java) to match the IPs for your local instances.

![alt text](https://raw.githubusercontent.com/itma96/proiect-sosm/master/Catalog%20App.png)

