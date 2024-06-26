# Read Me First

The original idea is from  
https://medium.com/itnext/reduce-the-startup-time-and-memory-footprint-of-your-java-app-by-20-49fc530f9c9d?source=explore---------1-109--------------------eb845d95_c32d_426e_95e3_35ab26b95768-------15

# Class Data Sharing (CDS)

The original idea is from  
https://digma.ai/top-features-in-spring-boot-3-2-part2/?__hstc=43953530.681dd9866de6b261d981ce95ae4ab937.1719386067577.1719386067577.1719386067577.1&__hssc=43953530.1.1719386067577&__hsfp=1926441786&_gl=1*16jdtli*_gcl_au*ODM2OTU0ODIyLjE3MTkzODYwNjg.*_ga*NDEwODM0Nzg1LjE3MTkzODYwNjc.*_ga_GP3SNPSMVW*MTcxOTM4NjA2Ny4xLjAuMTcxOTM4NjA2Ny42MC4wLjA.

Class Data Sharing (CDS) is a feature of the Java Virtual Machine (JVM) that can help decrease Java applications’
startup time and memory footprint. Starting in version 3.3, it was integrated into Spring Boot.

The CDS feature comprises two main steps:

1. Creating the CDS Archive, which creates an archive file (with .jsa format)
   containing the application classes when the application exits
2. Using the CDS Archive, which loads the .jsa file into memory.

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
