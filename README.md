# Lab 04 ARSW

This programm allow the user to make multiple requests at the same time using threads
2024/06/24


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

First you need the following java version (command to see your current java version below)

```
java -version
```

![image](https://github.com/Parralol/Taller1ARSW/assets/110953563/6088e13f-2c49-4e5f-9eb3-c09642af5d65)

to see the maven version we are using we need to enter the following command, also this is the version of Maven this programm uses

```
mvn -version
```

![image](https://github.com/Parralol/Taller1ARSW/assets/110953563/0c2f20e7-a955-4aa5-bb92-a073488ba7e1)

### Installing

First clone this proyect into your own system, then 

```
mvn clean package
```

### Acceptance test

this acceptance test is build around the following files which you can see here -> [file used](https://github.com/Parralol/Lab04/tree/main/src/main/java/edu/escuelaing/arsw/ase/app/resources)


![image](https://github.com/Parralol/Lab04/assets/110953563/02efe40d-9b23-44c9-a047-3450d49cf0cc)

as we can see here it takes three requests before shutting down.

![image](https://github.com/Parralol/Lab04/assets/110953563/8c378bbc-80cf-4b36-b6ef-ccb48f2d827b)

here we can see how the three different windows get the corresponging messages from the server, giving the same answer to them


## Deployment

**IN ORDER FOR THIS PROGRAM TO WORK, YOU'LL NEED TO EXECUTE THE PROGRAM ON THE FOLDER YOU WANT TO WORK WITH, WITH THE FILES YOU WANT TO WORK WITH**

if you want to use te programm before using the package command we use

```
mvn -e exec:java -Dexec'.mainClass=edu.escuelaing.arsw.ase.app.ConcurrentWebApp.java'
```
or (depending on your system)

```
mvn -e exec:java -Dexec.mainClass=edu.escuelaing.arsw.ase.app.ConcurrentWebApp.java
```

after the server has initialized, you'll have to type in the browser

http://localhost:35000

three times in order for something to show up

for each three submits to the server, the server WILL shutdown, be advised to start it each time


## Built With

* [Maven](https://maven.apache.org/) - Dependency Management
* [Java](https://www.oracle.com/java/technologies/) - Programming Language

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Santiago Parra** - *Initial work* - [Parralol](https://github.com/Parralol)
