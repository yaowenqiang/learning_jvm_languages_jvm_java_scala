```bash

javac -sourcepath src -d bin src/com/example/app/Controller.java
cd bin;
java  com.example.app.Controller

# class path


# ; for windows and : for linux and mac

java -cp ".;../lib" com.example.app.Controller
java -cp ".:../lib" -verbose:class com.example.app.Controller
java -cp ".:../lib" -verbose:gc com.example.app.Controller
java -cp ".:../lib" -verbose:jni com.example.app.Controller

https://dzone.com/articles/how-use-verbose-options-java



jps 
jinfo pidofjps
javap
```
