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

Java does a lot of crazy runtime optimizations so I was interested in
looking at the byte code. That and I had too much time in hand.

* Get the java 7 installed. I don't think this works on java 6 but who
uses java 6 anyway :).
* Get hsdis lib from
http://kenai.com/downloads/base-hsdis/hsdis-amd64.dylib
* Add the lib to your LD_LIBRARY_PATH
* Get rocking to look at the assembly code jit generates when it
executes your program.

$ java -XX:+UnlockDiagnosticVMOptions -XX:+PrintAssembly -cp . MyProgram

Now off to debug crazy assembly code looking at all the mov rax, rbx to
squeeze out last of performace from processor :). 

You can actually specify the assembly which you want it print out by
specifying +PringAssembly=intel.

And one more thing.. If you wanna disassembler for normal
binary in osx, it is not objdump but otool which does that. I know.. osx
right.



