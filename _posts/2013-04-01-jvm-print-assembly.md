---
layout: post
title: Enable JVM to print assembly code in osx
tags: jvm bytecode osx
year: 2013
month: 4
day: 1
published: true
summary: Print Java bytecode in osx
---

* Get the java 7 installed. I don't think this works on java 6 but who
uses java 6 anyway :).
* Get hsdis lib from
http://kenai.com/downloads/base-hsdis/hsdis-amd64.dylib
* Add the lib to your LD_LIBRARY_PATH
* Get rocking to look at the assembly code jit generates when it
executes your program.

java -XX:+UnlockDiagnosticVMOptions -XX:+PrintAssembly -cp . MyProgram






