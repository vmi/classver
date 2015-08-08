classver
========

This print Java class file version specified class files and/or jar files.

Usage
-----

    $ classver target/classes/hello/Hello.class
    Java 6.0 (50.0): target/classes/hello/Hello.class


    $ classver ~/.m2/repository/org/apache/ant/ant/1.9.6/ant-1.9.6.jar
    * Get class file name from jar.
    * Extract class file.
    Java 5.0 (49.0): /Users/vmi/.m2/repository/org/apache/ant/ant/1.9.6/ant-1.9.6.jar


    $ cd ~/git/selenese-runner-java
    $ mvn -Dmdep.outputFile=/tmp/classpath dependency:build-classpath
    (snip)
    $ classver $(cat /tmp/classpath) | tee /tmp/classver.list
    (snip)
    $ sort /tmp/classver.list
    Java 1.1 (45.3): /Users/vmi/.m2/repository/cglib/cglib-nodep/2.1_3/cglib-nodep-2.1_3.jar
    Java 1.1 (45.3): /Users/vmi/.m2/repository/org/w3c/css/sac/1.3/sac-1.3.jar
    Java 1.1 (45.3): /Users/vmi/.m2/repository/xalan/xalan/2.7.2/xalan-2.7.2.jar
    Java 1.1 (45.3): /Users/vmi/.m2/repository/xml-apis/xml-apis/1.4.01/xml-apis-1.4.01.jar
    Java 1.2 (46.0): /Users/vmi/.m2/repository/asm/asm/3.3.1/asm-3.3.1.jar
    Java 1.2 (46.0): /Users/vmi/.m2/repository/commons-collections/commons-collections/3.2.1/commons-collections-3.2.1.jar
    Java 1.3 (47.0): /Users/vmi/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar
    Java 1.3 (47.0): /Users/vmi/.m2/repository/net/sourceforge/nekohtml/nekohtml/1.9.22/nekohtml-1.9.22.jar
    Java 1.3 (47.0): /Users/vmi/.m2/repository/org/json/json/20080701/json-20080701.jar
    Java 1.3 (47.0): /Users/vmi/.m2/repository/xalan/serializer/2.7.2/serializer-2.7.2.jar
    Java 1.3 (47.0): /Users/vmi/.m2/repository/xerces/xercesImpl/2.11.0/xercesImpl-2.11.0.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/com/google/code/gson/gson/2.3.1/gson-2.3.1.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/com/googlecode/java-diff-utils/diffutils/1.3.0/diffutils-1.3.0.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/commons-cli/commons-cli/1.3.1/commons-cli-1.3.1.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/io/netty/netty/3.9.9.Final/netty-3.9.9.Final.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/junit/junit/4.12/junit-4.12.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/net/sourceforge/cssparser/cssparser/0.9.16/cssparser-0.9.16.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/net/sourceforge/htmlunit/htmlunit-core-js/2.17/htmlunit-core-js-2.17.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/org/apache/commons/commons-exec/1.3/commons-exec-1.3.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/org/hamcrest/hamcrest-all/1.3/hamcrest-all-1.3.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/org/littleshoot/dnsjava/2.1.3/dnsjava-2.1.3.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.12/jcl-over-slf4j-1.7.12.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/org/slf4j/jul-to-slf4j/1.7.12/jul-to-slf4j-1.7.12.jar
    Java 5.0 (49.0): /Users/vmi/.m2/repository/org/slf4j/slf4j-api/1.7.12/slf4j-api-1.7.12.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/ch/qos/logback/logback-classic/1.1.3/logback-classic-1.1.3.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/ch/qos/logback/logback-core/1.1.3/logback-core-1.1.3.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/com/codeborne/phantomjsdriver/1.2.1/phantomjsdriver-1.2.1.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/com/floreysoft/jmte/3.1.1/jmte-3.1.1.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/com/google/guava/guava/18.0/guava-18.0.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/net/java/dev/jna/jna-platform/4.1.0/jna-platform-4.1.0.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/net/java/dev/jna/jna/4.1.0/jna-4.1.0.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/org/apache/commons/commons-lang3/3.4/commons-lang3-3.4.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/org/apache/httpcomponents/httpclient/4.4.1/httpclient-4.4.1.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/org/apache/httpcomponents/httpcore/4.4.1/httpcore-4.4.1.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/org/apache/httpcomponents/httpmime/4.4.1/httpmime-4.4.1.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/org/littleshoot/dnssec4j/0.1/dnssec4j-0.1.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/org/littleshoot/littleproxy/0.5.3/littleproxy-0.5.3.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/jetty-rc-repacked/5/jetty-rc-repacked-5.jar
    Java 6.0 (50.0): /Users/vmi/.m2/repository/org/webbitserver/webbit/0.4.15/webbit-0.4.15.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/net/sourceforge/htmlunit/htmlunit/2.17/htmlunit-2.17.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/eclipse/jetty/jetty-io/9.2.11.v20150529/jetty-io-9.2.11.v20150529.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/eclipse/jetty/jetty-util/9.2.11.v20150529/jetty-util-9.2.11.v20150529.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/eclipse/jetty/websocket/websocket-api/9.2.11.v20150529/websocket-api-9.2.11.v20150529.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/eclipse/jetty/websocket/websocket-client/9.2.11.v20150529/websocket-client-9.2.11.v20150529.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/eclipse/jetty/websocket/websocket-common/9.2.11.v20150529/websocket-common-9.2.11.v20150529.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-api/2.47.1/selenium-api-2.47.1.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-chrome-driver/2.47.1/selenium-chrome-driver-2.47.1.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-edge-driver/2.47.1/selenium-edge-driver-2.47.1.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-firefox-driver/2.47.1/selenium-firefox-driver-2.47.1.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-htmlunit-driver/2.47.1/selenium-htmlunit-driver-2.47.1.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-ie-driver/2.47.1/selenium-ie-driver-2.47.1.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-leg-rc/2.47.1/selenium-leg-rc-2.47.1.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-remote-driver/2.47.1/selenium-remote-driver-2.47.1.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-safari-driver/2.47.1/selenium-safari-driver-2.47.1.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-server/2.47.1/selenium-server-2.47.1.jar
    Java 7.0 (51.0): /Users/vmi/.m2/repository/org/seleniumhq/selenium/selenium-support/2.47.1/selenium-support-2.47.1.jar
