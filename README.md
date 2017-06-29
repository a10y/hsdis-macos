# hsdis macOS

hsdis is a plugin for the HotSpot Oracle JVM that allows you to print out the assembly of JIT'ed calls.

Instructions for installing are below.

## Installation: JDK 1.8

```
cd $JAVA_HOME/jre/lib/server
wget https://raw.githubusercontent.com/a10y/hsdis-macos/master/hsdis-amd64.dylib
```

## Installation: JDK 1.9

```
cd $JAVA_HOME/lib/server
wget https://raw.githubusercontent.com/a10y/hsdis-macos/master/hsdis-amd64.dylib
```

## Usage

Assuming we have classfile `Main.class` present, a simple usage that works on JDK 1.8 and 1.9:

```
java -XX:+UnlockDiagnosticVMOptions -XX:+PrintAssembly Main
```
