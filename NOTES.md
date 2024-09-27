## Reasons for developing on JVM


### Java Class Library and ecosystem

+ Specific JVM version has specific classes
+ Java Class Library(SE 8)
  + Large collection of classes
  + JVM of SE 8 must implement these classes


### Java Class Library/Functionalities

+ Writting/reading from console window
+ Perform file I/O
+ TCP servers communication
+ Starting and managing OS threads
+ Defining data structures
+ Important reason for JVM popularity
+ Focused more on language design
+ incompartable and difficult to build from scrach

## Ecosystem

### Frameworks

+ Java Enterprise Edition(Java EE) (Oracle)
+ Spring framework echosystem

### Popular Application servers

open source 

+ Apache Tomcat
+ Apache TomEE
+ Red Hat WildFly
+ Orache GlassFish

per priority

+ Red Hat JBoss 
+ Oracle Weblogic


### High-level Web Application Framework

+ High-level APIs
+ Built-in model-view-controller(MVC) - enhance developer's productivity
+ Dictate or steer developer
+ Built-in support for few hardcode libraies/toolkits
+ Quick development cycles
+ Application run inside JVM application server/own HTTP server


### Microservice Framework

+ Built-in HTTP server
+ Not out-of-the-box tools for libraries
+ Easier to mix-and-match
+ Multiple standalone web services(not a requirement)
+ Most commonly used - Vert.x and Spark Java

## Popular Use cases

+ Web applications
+ Big data
+ IoT

### JVM in web applications

+ focused on performance
+ Scalable across different servers
+ Predictable
+ Debugging and profiling tools available
+ Monitoring of JVM internals possible
+ Examples - Twitter, Amazon, Spotify, and Nexflix

### Analyzing Data

+ Searching for something
+ Looking for patterns
+ Calculating statistics
+ Data can be obtained from:
  + Data collected from web servers
  + Output obtained from external sensors
  + Legacy servers

### Big Data - Popular Technologies

+ Apache Hadoop
  + Storage of data
  + Data distribution to other servers
+ Apache Spark
  + Data streaming
  + Incoming data analysis

### IoT

+ Popular and common
+ Memory-constrained systems:
  + Java ME embedded platform
  + Commercial IoT devices
+ Device sparing memory:
  + Java Se embedded edition
  + Desktop GUIs for full user interaction












Web application senarios

## JVM - popular use cases

## JVM concepts

+ JVM concepts
  + Virtual Machine
  + Cmpilers
  + classes
  + Backword compatibility
+ Java editions

### JVM concepts

+ Virtual Machine
+ JIT compiler
+ Built-in primitive datatypes
+ Reference types
+ Garbage collector process
+ Built tools


Application - JVM instance in system memory


JIT compiler

+ Often called routine - compiled
+ Advantages:
  + Cross platform files
  + No waiting for native compiling
  + immediate execution

### Primitive Datatypes

| Java Name | Description and Size | Values(inclusive) | 
| ---------- | -------------------- | ----------------- |
byte | Signed byte (8 bits) | -128 ~ 127
short | Signed short integer (16 bits) | -32768 ~ 23767
int | Signed integer (32 bits) | -2**31  ~ 2**31-1
long | Signed long integer (64 bits) | -2**64 ~ 2**63-1
float | Single-precision floating point (32-bit) | Non-precise floating point values
double | Double-precision floating point(64-bit) | Non-precise floating point values
char | A single Unicode UTF-16 character(16-bit) | Unicode character 0 to 65535
boolean | Boolean | True / False

https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html

### Java class library

+ Wrapper objects
  + Primitive types
  + languages
+ Autoboxing

### Classes

+ Contains functions and variables
+ Single-inheritance model
+ interface:
  + List of function prototypes and constants
  + Compiler has implementation for functions
+ Class grouped in packageso

### Refreence types


+ Refreence variable - points to specific instance or nothing
+ Specific instance:
  + Call object's methods
  + Access public atributes
+ Nothing
  + Null refreence


```java

Product p = new Product();
p.setName("box of biscuits");


p = null;
p.setName("This line will produce an error at run-time")



```

### Garbage Collector

+ In JVM
  + No manual allocation and release
  + Concentrate on ceating objects
+ Halts applications
+ Scans Memory
+ Remove objects deleted safely
+ Reclaim freed space
+ Configurable parameters for better control
+ Avoid creating tons of objects

### Trick to Tame GC

+ Put objects in a pool
+ One object plucked acrooding to need
+ Object put back when not needed                                                        


## Java editions

+ Java Standard Edition(Java SE)
+ Java Enterprise Edition(Java EE)
+ Java Micro Edition(Java ME)

### Java EE

+ Builds upon Java SE
+ Adds lot of APIs
+ Run inside JVM application servers
+ important addition for business developers
+ Download a full application server compatible with Java EE platform
+ APIs must be available                                                         


### Java ME

+ Important platform before android and IOS
+ Featured subset of Java-Class Library
+ Additional APIs
+ Java ME embedded - commercial IoT devices


## Other languages on JVM

