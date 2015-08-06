classver
========

This print class file version specified class file or jar file.

Usage
-----

    classver target/classes/hello/Hello.class

    classver ~/.m2/repository/org/apache/ant/ant/1.9.6/ant-1.9.6.jar

    mvn -Dmdep.outputFile=/tmp/classpath dependency:build-classpath
    classver $(cat /tmp/classpath) | tee /tmp/classver.list
    sort /tmp/classver.list
