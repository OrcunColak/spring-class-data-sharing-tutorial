# Read Me First

The original idea is from  
https://medium.com/itnext/reduce-the-startup-time-and-memory-footprint-of-your-java-app-by-20-49fc530f9c9d?source=explore---------1-109--------------------eb845d95_c32d_426e_95e3_35ab26b95768-------15

# Uber Jar

```
mvn clean package -DskipTests
java -jar target\spring-class-data-sharing-tutorial-0.0.1-SNAPSHOT.jar
```

# Class Data Sharing (CDS)  Jar

Extract the uber jar. This will create a new spring-class-data-sharing-tutorial-0.0.1-SNAPSHOT directory

```
java -Djarmode=tools -jar target\spring-class-data-sharing-tutorial-0.0.1-SNAPSHOT.jar extract
java -jar .\spring-class-data-sharing-tutorial-0.0.1-SNAPSHOT\spring-class-data-sharing-tutorial-0.0.1-SNAPSHOT.jar
```
