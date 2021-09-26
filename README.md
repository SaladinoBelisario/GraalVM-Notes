# **`GraalVM-Notes`**

# **Table of contents**

- [**Intro to JVM**](#intro-to-jvm)
  - [**Evolution of Java Virtual Machine**](#evolution-of-java-virtual-machine)
    - [Introduction to GraalVM](#introduction-to-graalvm)
    - [How JVM works](#how-jvm-works)
    - [Understanding the JVM architecture](#understanding-the-jvm-architecture)
  - [**JIT, HotSpot, and GraalJIT**](#jit-hotspot-and-graaljit)
    - [Taking a deep dive into HotSpot and the C2 JIT compiler](#taking-a-deep-dive-into-hotspot-and-the-c2-jit-compiler)
    - [Understanding the optimizations performed by JIT](#understanding-the-optimizations-performed-by-jit)
    - [Deoptimization](#deoptimization)
    - [Graal JIT and the JVM Compiler Interface (JVMCI)](#graal-jit-and-the-jvm-compiler-interface-jvmci)
- [**GraalVM – Architecture and Implementation**](#graalvm--architecture-and-implementation)
  - [**GraalVM architecture**](#graalvm-architecture)
    - [Reviewing modern architectural requirements](#reviewing-modern-architectural-requirements)
    - [Learning what the GraalVM architecture is](#learning-what-the-graalvm-architecture-is)
    - [Reviewing the GraalVM editions (Community and Enterprise)](#reviewing-the-graalvm-editions-community-and-enterprise)
    - [Understanding the GraalVM architecture](#understanding-the-graalvm-architecture)
    - [An overview of GraalVM microservices architecture](#an-overview-of-graalvm-microservices-architecture)
    - [Understanding how GraalVM addresses various nonfunctional aspects](#understanding-how-graalvm-addresses-various-nonfunctional-aspects)
  - [**Graal Just-In-Time Compiler**](#graal-just-in-time-compiler)
    - [Understanding the Graal JIT compiler](#understanding-the-graal-jit-compiler)
    - [Understanding Graal compiler optimizations](#understanding-graal-compiler-optimizations)
  - [**Graal Ahead-of-Time Compiler and Native Image**](#graal-ahead-of-time-compiler-and-native-image)
    - [Building native images](#building-native-images)
    - [Analyzing the native image with GraalVM Dashboard](#analyzing-the-native-image-with-graalvm-dashboard)
    - [Understanding PGO](#understanding-pgo)
    - [Native image configuration](#native-image-configuration)
    - [Generating Graal graphs for native images](#generating-graal-graphs-for-native-images)
    - [Understanding how native images manage memory](#understanding-how-native-images-manage-memory)
    - [Building static native images and native shared libraries](#building-static-native-images-and-native-shared-libraries)
    - [Debugging native images](#debugging-native-images)
    - [Limitations of Graal AOT (Native Image)](#limitations-of-graal-aot-native-image)
    - [GraalVM containers](#graalvm-containers)
- [**Polyglot with Graal**](#polyglot-with-graal)
  - [**Truffle – An Overview**](#truffle--an-overview)
    - [Exploring the Truffle language implementation framework](#exploring-the-truffle-language-implementation-framework)
    - [Exploring the Truffle interpreter/compiler pipeline](#exploring-the-truffle-interpretercompiler-pipeline)
    - [Learning Truffle DSL](#learning-truffle-dsl)
    - [Understanding how Truffle supports interoperability](#understanding-how-truffle-supports-interoperability)
    - [Understanding Truffle instrumentation](#understanding-truffle-instrumentation)
    - [Ahead-of-time compilation using Truffle](#ahead-of-time-compilation-using-truffle)
    - [Optimizing Truffle interpreter performance with launcher options](#optimizing-truffle-interpreter-performance-with-launcher-options)
    - [SimpleLanguage and Simple Tool](#simplelanguage-and-simple-tool)
  - [**Language interoperability**](#language-interoperability)
    - [Understanding the JavaScript (including Node.js) Truffle interpreter](#understanding-the-javascript-including-nodejs-truffle-interpreter)
    - [Understanding Espresso (Java on Truffle)](#understanding-espresso-java-on-truffle)
    - [Understanding GraalPython – the Python Truffle interpreter](#understanding-graalpython--the-python-truffle-interpreter)
    - [Understanding LLVM – the (Sulong) Truffle interface](#understanding-llvm--the-sulong-truffle-interface)
    - [Understanding GraalWasm – the WASM Truffle interpreter](#understanding-graalwasm--the-wasm-truffle-interpreter)
- [**Microservices with Graal**](#microservices-with-graal)
  - [**Microservices Architecture with GraalVM**](#microservices-architecture-with-graalvm)
    - [Overview of microservices architecture](#overview-of-microservices-architecture)
    - [Building microservices' architecture with GraalVM](#building-microservices-architecture-with-graalvm)
    - [Case study – online book library](#case-study--online-book-library)
    - [Exploring modern microservices frameworks](#exploring-modern-microservices-frameworks)

# **Intro to JVM**

## **Evolution of Java Virtual Machine**

### Introduction to GraalVM
### How JVM works
### Understanding the JVM architecture

## **JIT, HotSpot, and GraalJIT**

### Taking a deep dive into HotSpot and the C2 JIT compiler
### Understanding the optimizations performed by JIT
### Deoptimization
### Graal JIT and the JVM Compiler Interface (JVMCI)  

# **GraalVM – Architecture and Implementation**

## **GraalVM architecture**

### Reviewing modern architectural requirements
### Learning what the GraalVM architecture is
### Reviewing the GraalVM editions (Community and Enterprise)
### Understanding the GraalVM architecture
### An overview of GraalVM microservices architecture
### Understanding how GraalVM addresses various nonfunctional aspects  

## **Graal Just-In-Time Compiler**

### Understanding the Graal JIT compiler
### Understanding Graal compiler optimizations  

## **Graal Ahead-of-Time Compiler and Native Image**

### Building native images
### Analyzing the native image with GraalVM Dashboard
### Understanding PGO
### Native image configuration
### Generating Graal graphs for native images
### Understanding how native images manage memory
### Building static native images and native shared libraries
### Debugging native images
### Limitations of Graal AOT (Native Image)
### GraalVM containers  

# **Polyglot with Graal**

## **Truffle – An Overview**

### Exploring the Truffle language implementation framework
### Exploring the Truffle interpreter/compiler pipeline
### Learning Truffle DSL
### Understanding how Truffle supports interoperability
### Understanding Truffle instrumentation  
### Ahead-of-time compilation using Truffle  
### Optimizing Truffle interpreter performance with launcher options  
### SimpleLanguage and Simple Tool

## **Language interoperability**

### Understanding the JavaScript (including Node.js) Truffle interpreter
### Understanding Espresso (Java on Truffle)
### Understanding GraalPython – the Python Truffle interpreter
### Understanding LLVM – the (Sulong) Truffle interface
### Understanding GraalWasm – the WASM Truffle interpreter

# **Microservices with Graal**

## **Microservices Architecture with GraalVM**

### Overview of microservices architecture
### Building microservices' architecture with GraalVM
### Case study – online book library
### Exploring modern microservices frameworks
