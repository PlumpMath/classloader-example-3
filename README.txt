Pankaj$ javac -cp . com/journaldev/cl/Foo.java
Pankaj$ javac -cp . com/journaldev/cl/Bar.java
Pankaj$ javac CCLoader.java
Pankaj$ javac CCRun.java
CCRun.java:18: warning: non-varargs call of varargs method with inexact argument type for last parameter;
cast to java.lang.Class<?> for a varargs call
cast to java.lang.Class<?>[] for a non-varargs call and to suppress this warning
Method printCL = clas.getMethod("printCL", null);
^
1 warning
Pankaj$ java CCRun com.journaldev.cl.Foo 1212 1313
Loading Class 'com.journaldev.cl.Foo'
Loading Class using CCLoader
Loading Class 'java.lang.Object'
Loading Class 'java.lang.String'
Loading Class 'java.lang.Exception'
Loading Class 'java.lang.System'
Loading Class 'java.lang.StringBuilder'
Loading Class 'java.io.PrintStream'
Foo Constructor >>> 1212 1313
Loading Class 'com.journaldev.cl.Bar'
Loading Class using CCLoader
Bar Constructor >>> 1212 1313
Loading Class 'java.lang.Class'
Bar ClassLoader: CCLoader@71f6f0bf
Foo ClassLoader: CCLoader@71f6f0bf
ctk-pcs1313512-2:src pk93229$