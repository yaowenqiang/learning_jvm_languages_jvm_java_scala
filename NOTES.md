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

### Reference types


+ Reference variable - points to specific instance or nothing
+ Specific instance:
  + Call object's methods
  + Access public atributes
+ Nothing
  + Null reference


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

### JVM Specification Documentation

+ Low-level commands JVM can execute
+ Required data structures
+ Accessing emory rules
+ Java bytecode's .class format
+ Enabled writers to experiment

### Mixing languages

+ languages offer interoperability with JVM languages
+ Use of standard Java Class Library classes for data structures
+ Compile methods similar to Java
+ Certain classes compiled in different languages
+ Complicates process

### Writting Unit Tests in different languages

+ common to test Java code with unit tests of different languages
+ Code in other languages:
  + Compact
  + ideal for small, concrete and readable unit tests
  + Language's runtime library only used while executing
  + Not bundle with compiled main project
+ Groovy:
  + Built-in assert statement
  + Prints verbose and readable output

## Install 

env 

> JAVA_HOME

https://docs.oracle.com/javase/8/docs/api/

JDK - Important Components

| Directory Name | Description | 
| ---------------- | ----------- |
| bin | Contains all the executable commands that are supplied with JDK | 
| db | Everything related to the JavaDB component is stored here. JavaDB is Oracle's supported version of the Apache Derby database project.Derby is an open source file-based relational database system that has strong SQL support. it is fully implement in java.| 
| include | For advanced programmers. contains headers for C compilers that can be used to call platform - or operation-system-specific native code from java code or vice versa.| 
| jre | files related to JRE stored,including Java Class Library, All the commands from the jre/bin directory are also placed in JDK's bin subdirectory|
| lib | Libraries used by certain development tools are stored here.|



JDK - Commands

| Directory Name | Description | 
| ---------------- | ----------- |
| jar | This is the tool to creat a new, extract data from, or add files to existing JAR archive files. | 
| jarsigner | This protects JAR files by adding a digital signature to them. if the data inside a JAR file is modified without updating the signature, it will no longer be considered valid.| 
| jdeps | This outputs dependency information of a JVM-compiled .class file or a JAR file.| 
| jjs | This launchs Oracle Nashorn's interactive interpreter shell. Nashorn is Oracle's JavaScript interpreter |


https://www.oracle.com/technical-resources/articles/java/jf14-nashorn.html

GUI Monitor Tools

+ Commands that offer a fuul desktop GUI:
  + Java VirtualVM
  + Oracle Misson Control
  + JConsule

Java VisualVM

+ included in Oracle's JDK and open source OpenJDK
+ Monitors JVM instances of each running JVM application
+ Built-in features enhanced by installing plugins

https://visualvm.github.io/

> jvisualvm


Oracle Misson Control

+ Present in Oracle's recent JDK version
+ Monitors JVM instances and running application
+ Better user interface than Java VirtualVM
+ Propriety software
+ Java Flight Recorder(free in development environment)


> jmc

JConsole

+ Oldest monitoring tool
+ Other tools are better

> jconsole


JRE

+ Installs the Java command
  + Runs JVM instance and full Java Class Library
+ Used to start applications

+ JRE
  + 32-bit or 64-bit
  + End user desktop machines
+ Server JRE
  + Servers by advanced system admins
  + 64-bit

## Class Organization with Packages

### Rule for Package Names

+ Package name can have dots
+ Dots used to separate element
+ Element - letters, digit, underscore
+ Element must start with letter
+ Element connot be same as keyword (int, short, class, for, final)

### Universal Naming Conventions

+ Package name in lowercase
+ Start package name with reversed internet URL of:
  + Company's site
  + Project's site
  + Project's public source code repository
  + Personal home page
+ Own convention to differentiate classes and prevent naming conflicts
+ illegal element:
  + Put an underscore before of after it 
  + Replace the illegal character with underscore

## Java Class Library

Java class library

+ Also known as Java API
+ Collection of pre-built Classes

Common data structures - definitions and implementations

+ Console I/O
+ File I/O
+ GUI Toolkits
+ Networking
+ Regular expressions
+ XML creation and processing
+ Database Access
+ Reflection
+ Mathematics


#### Packages

+ All classes in library
+ Important packages names start with java or javax
+ Vendor's clases are in packages starting with:
  + com.sun, sun or com.oracle
+ Using add-on libraries recommanded

#### Most important packages

| Package(s) | Description |
| ---------- | ----------- |
| java.lang | This class is considered fundamental, it contains the String and StringBuilder classes, primitive wrappers, threading, and the mother of all objects - Object. |
| java.lang.reflect | This offers APIs for reflection. Reflection make it possible to dynamically look at classes to look up method and variable names, invoke methods, and read or write atributes | 
| java.util | This is on of the most important packages,it contains classes that implement collections, dat and time, internationalization, and many others.|
| java.util.cuncurrent | This contains classes for concurrent programming |
| java.io | ---- |
| java.net | ---- |
| java.nio | These are classes for the operation system, file, and networking I/O. it also contains character-set encoding/decoding classes. |
| java.math | This offers the BigDecimal class.which is much more precise than the primitive float and double types and the BigInteger class, which can hold larger values than the int and long primitive types |
| java.xml | This refers to the XML processing classes |
| java.sql, |  --- |
| javax.sql, | this contains classes to work with the JDBC database system. |
| javax.awt, | this is Abstract Window Toolkit. the earliest Java GUI toolkit. It offers a layer between the native GUI of the operation system and the JVM.|
| java.swing | This refers to the Swing GUI toolkit classes. built on top of the AWT toolkit. A big difference with AWT is that all the GUI controls are implement in the Java cod in them. |
| javafx | This refers to the JavaFX GUI toolkit classes. This is a very modern offering of 3D accelerated graphics. |

Commonly used Methods of java.lang.Object

| Method Name | Return Type | Description | 
| ----------- | ----------- | ----------- |
| toString()  | String      | This returns the textual description of the object |
| equals(Object object)  | Boolean | This returns whether the passed object is considered equal to the current object |
| hashCode() | int | This is called when a hash value of the current class is required |

String Class - java.lang.String


+ Represents JVM string type
+ Changes to string object do not change original object
+ Produces a new string with modified content
+ Stored internally in UTF-16 encoding

### Need of Primitive Wrapper classes

+ All APis cannot work with built-in primitive datatypes
+ If primitive wrapper class is required, corresponding instance created
+ Primitive variable required, wrapper object assigned:
  + Value of wrapper class assigned to primitive variable.

### Exceptions and Errors

+ Handling runtime errors different in different languages
+ Built-in classes inheriting Exception or Error class
+ Look for an exception that can be reused
+ Example - method not excepting null references throws:
  + java.lang.NullPointerException

### Distiction between Exception and Error

| Exception  | Error | 
--- | ---
thrown when the program can handle the error and continue running | Problem detected that can not be anticipaged.


### Exceptions 


+ Java bytecode - comiles source code file names and line numbers
+ Advantage - source code line numbers returns to stack trace
+ Readable stack traces
+ In Java, not all classes can throw all exceptions

### Collections API

+ java.util package -data structures
+ Use own variations for additional functionality
+ Maximal compatibility with :
  + Java and JVM platforms with built-in classes
+ Collection classes only work with objects
+ Primitive values autoboxed into object and vice versa
+ Collection classes:
  + java.util.ArrayList - a list class
+ java.util.HashMap - container for key/value combination

| Collections Classes | Python | Ruby |
--- | ---- | ---
java.util.ArrayList | List type | Array object 
java.util.HashMap | Dict type | Hash object 

#### ArrayList

+ implements List structure that hold other objects
+ Easier to work with
+ Advantages:
  + Grows automatically when more space is needed
  + Lot of methods to calculate size of array
  + Methods are also added by some languages

#### HashMap

+ Store key/value combination - map
+ inserting objects - key  object and value object specified
+ Value object retrived with the help of key object
+ Original order of keys not kept


#### HashMap - Methods

| Method Name | Return Type | Description | 
| ------ | ----- | ---- |
put(Object key, Object value) | Object | This is to add a new key and value pair. if the key already exists, then the corresponding value is overwritten with the passed value. it returns null if the key is already added , otherwise, it returns the existing value
putAll(Map map) | This add all the key/value pairs from the specified map , again overwriting values when the keys already exist.
| containsKey(Object key) | Object | This returns whether the key is currently in the map
| get(Object key) | Object | This returns the value associated with the key. or it returns null when the key is not found
| getOrDefault(Object key, Object defaultValue) | Object | This returns the associated value if the key can be found, otherwise, it returns the passed defaultValue
| clear() | - | This empties the collection; all the key/value paires will be removed
| Size() | int | This returns the number of key/value pairs that the Map currently stores


#### java.lang.Object Methods

+ hashCode
+ equals
+ Java - define classes and write implementations for both methods
+ Other languages - generate implementations automatically
+ Can override JVM's automatically generated methods

### hashCode()

+ Called when a hash of the object is needed
+ Returns integer value when object content Changes
+ Returns a value disticnt from other similar objects

## Running JVM Applications on the Command Line


Introduction

+ Running application is complex
+ Source codes compiled to binary files with a .class file extension
+ Rules:
  + At least one class must have static main method
  + Class files should be stored in specific directories
  + ClassPath has to be specified
  + Java command used to run the program

Points to Remember

+ Avoid having classes in project outside package
+ Compiler creates the correct directory structure automatically
+ Compilers require source to be organized according to requirements


ClassPath

+ List of directories used by JVM to find refreenced class
+ Defaults to current directory unless set
+ Don't set ClassPath explicitly if:
  + All files used are stored in directory used to launch program
  + Class file package name matches the directory structure

Add-On Libraries

+ Used often in the real world
+ Runtime library required
+ Put add-on library files in separate directory
+ Library placed in JAR file - specify it on ClassPath

ClassPath

+ Absolute and relative paths specified for a JAR file
+ Relative paths:
  + Start point - directory from where command is launched
+ Entries read from left to right
+ Orders is important
+ Values of CLASSPATH environment set - taken
+ -cp or classpath command-line option specified on the java command - taken

### Placing Class Files inside a JAR Archive

+ Convenient
+ External dependencies required by JAR file put on ClassPath
+ Mentioned in Documentation

### Runnable JAR File

+ Can be started using java command
+ JAR file specifes the class that contains main method
+ Self-contained
+ Has all required dependencies
+ Main methods does not need to be pointed out
+ cannot find class placed outside the JAR file


## Java

### Naming Convention

+ CamelCase
+ Starts with a captial letter
+ No space between words
+ Each new word starts with a captial letter

### Rules for a Class Name

+ Starts with a non-digit character
+ No dashes and spaces
+ Digits are allowed after first letter
+ Keywrds not allowed

### Class Access Modifiers

+ Can be used to modify visibility
+ Default visibility - package private;
  + Can bee referenced to or instantiated by same package classes

### Defining Packages

+ Package - puts class inside package
+ First uncommented line in code 
+ Statement ends with semicolon
+ Example - com.example.package_name;

### Importing Classes

+ Not recommanded for larger systems
+ Classes from specified packages are imported
+ Example - java.util.concurrent:
  + Utility classes for concurrent programming
+ Import statements from both packages required
+ java.lang - packages imported implicitly

### Adding Variables and Methods

+ Variables hold data
+ Methods act upon data
+ Visibility chagned by using access Modifiers

### Initializing Values

+ implicit:
  + 0 - int, long, and short
  + 0.0 - float, double
  + False - Boolean
  + Null - refreence types

### Variable - Naming convention

+ Start with lowercase
+ Special characters not recommanded

### Methods

+ Method with return type - return the object or null
+ Method with void - not allowed to return anything 
+ Variables should be Initialized before using them

### Modifiers

+ Types:
  + Access Modifiers
  + Non-access Modifiers
+ While mixing, order not important
+ Convention - first access, then non-access
+ Class decides accessbility with the help of modifiers


#### Access Modifiers

| Name | Access Modifier | Description |
------ | ----------------| ------
Public | public  | Can be accessed by all parts of the code that have access to the class
Protected | protected | Can be seen and accessed by the class itself, other classes in the same package, and classes that inherit the class hidden from all other classes
Package-private | - | When you don't specify an access Modifier,the class member can only be seen and accessed by the class itself and other classes in the same package hidden from classes in other packages, even when such a class could inherit the class
Private | private | Only be seen and accessed by the class that defines the member

### Static Variable and Method

+ Variable - can be accessed without instance
+ Method - called without reference type

### Constructors and Finalizers

+ Defined by Java objects
+ Constructors called when class instance created
+ finalize() - when object to be collected by gargage Collector


### finalize()

+ Free resources that the class is utilizing
+ Close resources as early as possible to free finalize()
+ Can write a log when finalize() is used

### Constructor - Rules

+ Sublass Constructors call parent's constructor
+ No constructor in subclass:
  + Constructor required in parent class
+ No constructor with empty parameters in parent class:
  + Subclass constructors call parent class with valid parameters
+ Calls parent class's parameterless constructors automatically

### Abstract Class

+ Prefix - Abstract
+ Can be extended
+ Not instantiated

### Interfaces

+ Similar to abstract blass
+ Unable to provide implementations of methods
+ Implemented by classes

### Interfaces - Rules

+ Public interface should be defined in a file matching the interface name
+ Support public and Package-private
+ Members - implicitly abstract and public
+ Access modifiers explicitly added
+ Public modifiers only
+ Method - public instance methods
+ Variables - final and static modifiers
+ Class can implement any number of interfaces

### Why provide default implementations

+ Adding new methods broke compatibility
+ Classes had to be modified before compiling

### A new Feature

+ Adding static methods to an interface
+ implementations for static methods needs to be provided
+ Reference tyep variable will not provide access to static methods 


### Operators

| Operator | Description |
| --------- | -----
| value++ | - 
| value-- | Returns the value, then increase or decrease the value
| ++value | -
| --value | Increase or decrease the value,then returns the value
| ! | Logical NOT operator
| % | Refers to the remainder (integer) of a division
| instanceof | Returns a Boolean indicating wether the passed object is an instance of the specified clas or interface.
| == | -
| != | Refer to equal to and unequal to signs
| && | -
| !! | Logical AND or OR operations
| =  | Refers to an assignment
| +=, -=, *=, /=  | Calculate a new value and directly asign the resut to the variable

### Equals to (==)

+ Works properly on primitive variables
+ In objects, object references are compared
+ Class content is not compared
+ Consequence - content of a String variable checked with the equals methods


### POJO


A class is a POJO if

+ Does not extend classes or implement interfaces
+ Class is mutable
+ Public construction accepts on parameters

### POJO Property

+ A value that can be set and retrived using methods
+ Process：
  + Property values stored in private variables
  + Getter - return values
  + Setter - store values
  + Getter method prefix - get/is
  + Setter prefix - set

### Arrays

#### Points to Note

+ Arrays utility class - static, convenient utility methods
+ Consult API Documentation for:
  + Converting arrays into a collection class instance
  + Searching an item in array
  + Sorting the array

### Generics

+ Certain classes can be used with a fixed type
+ Example:
  + ArrayList storing java.lang.integer class instalce will refuse to compile others

### HashMap

+ Class from java.util package
+ Implements java.util.Map interface
+ Use for reference variable and to hide that we are using Hashmap

### Catch Blocks

+ None applicable - caller of methods
+ Try...catch block present  - analysis
+ Match found - control transfered
+ No try...catch block - look at caller till stack exhausts
+ No try...catch block handle - program will crash

### Catch Blocks - Order

+ Most concrete Exception classes
+ Exception subclasses
+ Exception


### Character Class

+ Wrap a char primitive value
+ Char - single quotes
+ String - double quotes
+ Get method - returns integer wrapper class comtaining frequency
+ AssertEquals(int, int) easily used
+ If mentioned version not used, casting required





## Install java jupter kernel

> brew install jbangdev/tap/jbang
> jbang install-kernel@jupyter-java
> jupyter lab

## Scala

> scala 

> https://docs.scala-lang.org/
> https://www.scala-lang.org/api/current/

### Functional Versus Imperative(命令式) programming

#### Imperative Programming

+ Multiple variables and classes with internal states
+ Example - PIJO(Plain Old Java Object)
+ POJO:
  + Variables can be changed by calling setter methods
  + Node reaching POJO instance can modify its variables
  + Can lead to bugs

#### Functional Progarmming

+ Existsing variables not mofified when code is running
+ Values specified as function parameters
+ Output generated based on parameters of values
+ Functions - return same output for same parameters

```scala
    class AddDemoOOP {
        var x = 0
        def add(y: Int) :INt = {
            x += y
            x
        }
    }
     class AddDemoFunctional {
        var x = 0
        def add(x:Int, y: Int) :INt = {
            x + y
        }
    }
```
### Functional Programming - Advantage

+ Popular with programs with multiple threads
+ Safer than Imperative code

## Scala Language syntax and Rules

### Scala - Statically Typed language

+ Declare variables before using them
+ Spcify used types
+ Types specified when declaring method imput parameters
+ Types not required when declaring variables inside a method or function body

```scala
var i = 10
var j = new java.lang.Object()
```

### Mutable and immutable Variables

+ Prefix with variables when declaring method parameters
+ var - muitable variables
+ val - fixed variables

+ Variable
  + Normal variables in java
  + Fully mutable
  + Freely changed
+ Fixed Variable
  + Final variables
  + Can be assigned only once
  + Content can be changed
+ immutable variables:
  + Functional Programming
  + immutable variables

### Common Scala Types

+ Any
+ AnyRef
+ AnyVal
+ Strings

### Any


+ Scala's parent class

### AnyRef

+ Used by reference variables
+ Similar to java.lang.Object
+ Methods - equals, hashCode, finalize

### AnyVal

+ Used by value classes
+ Has wrapper classes(primitive values) as subclasses


### Why Scala Has its Own Wrapper Class?

+ Improves performance
+ Uses internal Logical
+ Operator overloading

### Strings

+ Normal string class from java.lang package
+ immutable
+ String modified -> modified string instance returns
+ Perfect fit fot Scala's functional language

### OOP in Scala

+ Scala compiler requires code wrapped in class
+ Code automatically wrapped in invisible class by Repl
+ Immediately write function or code to execute

#### Defining Classes and Subclasses

+ More support
+ Packages having same prefixes are related
+ Define subpackage in same file that contains packages


```scala
package packagename
package com.example.parent

class A {

}

package subpackage {
class B {}
class C {}

}

```

#### REPL Shell


+ Package statement cannot be used
+ generates an invisible class that has code 
+ Compile source code with scalac compiler


```scala
import com.example.parent.A
import com.example.parent._
import com.example.parent.{B,C}
import com.example.parent.{C => D}

import com.example.parent
var c = new parent.subpackage.C()

class TheClassName {

}



```

#### defining Classes

+ Any numbers of classes defined
+ Source file name not require to match with classes it defines
+ Private access mofifier supported
+ Not specifying a modifier makes a class public

#### Instance Variables and Methods

+ Present in classes
+ Class methods and variables not supported in Scala
+ Singleton classes are the alternative
+ Instance variables
  + Added by defining def and val variables
  + Scala detects type from initialization

#### Instance Variables - initialization

+ Not to be initialized explicitly
+ Initialized with a null value
+ Value must be assigned at the time of declaration

#### Instance Methods

+ Method declaration similar to java
+ Types of input parameters need to be specified
+ Can return nothing on or instance
+ Return type - optional

```scala
def methodName(parameger1: Int, parameger2: Int): Int = {
    parameger1 + parameger2
}

```

#### Return Type

+ explicitly
+ Not require or recommended
+ When using return statement, explicitly define return type
+ Unit class name - method does not return anything


```scala
def methodWithoutReturnValue(): Unit = {

}

def helloWorld() = println("Hello world")

```

#### Access Modifiers

+ Class public when no access modifier
+ Other - protected and private
+ Scala:
  + Subpackage classes can access private members of parent package
  + Method with protected modifier - not visible to other Classes

#### constructor

```scala
class ClassWithParameterizedConstructor(var parm1: Int, param2: Int) {
    println("This code is executed as part of the constructor")
}

class ClassWithParameterizedConstructor(var parm1: Int, param2: Int) {
    def this(param1: Int) = this(param1,0)
}
```

#### Points to Note

+ Scala automatically creates fields for same name parameters
+ Getters and setters generated implicitly
+ Constructor parameters freely accessed
+ Between var and val, val is implicity chosen
+ All variables are values can be accessed  by all code
+ Statements in the body are executed when man constructor used
+ Constructors can be overloaded(Auxiliary constructors 辅助构造器)
+ Creating an additional construcotr - 'this'


```scala
class ClassWithParameterizedConstructor(val param1: Int, val param2: Int) {
    def this(param1: Int) {
        this(param1, 0)
    }
}

```


#### Rule for Auxiliary Constructors:

+ First line:
  + Call the primary constructor
  + Call one of the constructors defined before the current one

### Extending a Class

+ 'extends' keyword used
+ Inheritance of single class allowed
+ If no class inherited AnyRef class is
+ Only primary constructor of subclass can call parent class constructor

```scala
    class ParentClass {
    }
    class SubClass extends ParentClass {
    }
    class ParentClass(param1: Int, param2: Int) {
    }
    class SubClass(var param1: Int) extends ParentClass(param1, 10) {
    }

```

#### Override methods

```scala
class ParentClass {
def test() = print("Hellok, from the parent class")
}
class SubClass extends ParentClass {
override def test() = {
    super.test()
    print("Hellok, from the child class as well")
}
}

class OverloadExample {
def anOverloadMethod(i: Int) {}
def anOverloadMethod(s: String) {}
} 

abstract class AbstractClassName {
def methodWithNoImplementationYet
def methodWithImplementation() {}
} 

trait traitName {
def methodWithImplementation() {
}
def methodWithoutImplementation()
}

trait traitA {def method1()}
trait traitB {def method2()}
trait traitC {def method3()}

class TraitDemoClass extends TraitA with TraitB with TraitC {
def method1() {}
def method2() {}
def method3() {}
}

object SingletonObjectName {
var x = 100
def printX() = println(x)
}
SingletonObjectName.x = 250
SingletonObjectName.printX()

```

#### Operator overloading

+ In Java:
  + '+' and * cannot be overriden
+ IMplements operators as ordinary method
+ Possible to override operators and implement them in custom classes
+ For example:
  + Using the + method
  + '+' decides the operation depending on the instances

```java
class A (
public static void main (String[] args) {
    // compile error: bad operand types for binary operator '+'
    A result = new A() + new A();
}
)

```


```scala
class CustomClass(var x: Int) {
    def + (other: CustomClass) = {
        new CustomClass(x + other.x)
    }
}

val result = new CustomClass(400) + new CustomClass(500)

```

#### Case classes

```scala
abstract class Figure 
case clas Rectangle(x1: Int, y1: Int, x2: Int, y2: Int) extends Figure
case clas Circle(x: Int, y: Int, diameter: Int) extends Figure
case clas Line(x1: Int, y1: Int, x2: Int, y2: Int) extends Figure

val rectangle = Rectangle(10, 20,80 ,50)
val circle = Circle(100,200,30)

def drawFigure(figure: Figure) : Unit = {
    figure match {
        case Rectangle(x1, y1, _, _) => _draw(x1, y1)
        case Circle(x, y, _) => _draw(x, y)
        case Line(x1, y1, _, _) => _draw(x1, y1)
    } 
    def _draw(x:Int, y:Int) : Unit = println("Start drawing at " + x + ", " + y)
    
}

drawFigure(rectangle)
drawFigure(circle)

```

## Scala's standard Library

