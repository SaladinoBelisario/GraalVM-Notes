# **`GraalVM-Notes`**

# **INDEX:**

## Intro to JVM

### Evolution of Java Virtual Machine

- Introduction to GraalVM
- How JVM works
- Understanding the JVM architecture

### JIT, HotSpot, and GraalJIT

- Taking a deep dive into HotSpot and the C2 JIT compiler
- Understanding the
  optimizations performed by JIT
- Deoptimization
- Graal JIT and the JVM Compiler Interface (JVMCI)  

## GraalVM – Architecture and Implementation

### GraalVM architecture

- Reviewing modern architectural requirements
- Learning what the GraalVM architecture is
- Reviewing the GraalVM editions (Community and Enterprise)
- Understanding the GraalVM architecture
- An overview of GraalVM microservices architecture
- Understanding how GraalVM addresses various nonfunctional aspects  

### Graal Just-In-Time Compiler

- Understanding the Graal JIT compiler
- Understanding Graal compiler optimizations  

### Graal Ahead-of-Time Compiler and Native Image

- Building native images
- Analyzing the native image with GraalVM Dashboard
- Understanding PGO
- Native image configuration
- Generating Graal graphs for native images
- Understanding how native images manage memory
- Building static native images and native shared libraries
- Debugging native images
- Limitations of Graal AOT (Native Image)
- GraalVM containers  

## Polyglot with Graal

### Truffle – An Overview

- Exploring the Truffle language implementation framework
- Exploring the Truffle interpreter/compiler pipeline
- Learning Truffle DSL
- Understanding how Truffle supports interoperability
- Understanding Truffle instrumentation  
- Ahead-of-time compilation using Truffle  
- Optimizing Truffle interpreter performance with launcher options  
- SimpleLanguage and Simple Tool

### Language interoperability

- Understanding the JavaScript (including Node.js) Truffle interpreter
- Understanding Espresso (Java on Truffle)
- Understanding GraalPython – the Python Truffle interpreter
- Understanding LLVM – the (Sulong) Truffle interface
- Understanding GraalWasm – the WASM Truffle interpreter

## Microservices with Graal

### Microservices Architecture with GraalVM

- Overview of microservices architecture
- Building microservices' architecture with GraalVM
- Case study – online book library
- Exploring modern microservices frameworks
