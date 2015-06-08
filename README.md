# Java-Build-Script
A simple example for building executable jar

```bash
# -classpath后面填写jar包路径 -d后面填写源码路径
javac -classpath lib/* -d ./ src/recommend/search/*.java
# MANIFEST.MF文件放在当前目录下即可，想打成的jar包名称，class字节码文件路径
jar cvmf MANIFEST.MF demo.jar recommend/search/*.class
# 执行jar包
java -jar demo.jar
```
