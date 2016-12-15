# Protelis-Sandbox

A sandbox environment for debugging [Protelis](http://protelis.github.io/) code through [Alchemist Simulator](https://github.com/AlchemistSimulator/Alchemist)

## Requirements

To run the simulation [Java
  8](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html) is required

## Getting Started

These instructions describe how to set up and run the simulation

### Structure

How the simulation is structured

```
/protelis-sandbox/src/main/
|------> effects/ (Add effects to the simulation)
|------> protelis/ (Protelis code)
|------> resources/ (Maps, ...)
|------> yaml/ (Alchemist configurations)
```
### Dependencies

* Alchemist. Change `alchemistVersion` in `gradle.properties` to update the Alchemist release

### Modify and run the simulation

To execute the simulation
```
cd protelis-sandbox
./gradlew
```

Modify `simulation` in `gradle.properties` to change the simulation that will be executed. Note that by default simulation effects should have the same name of the simulation.

### Working with Eclipse

Writing Protelis code is way easier with Eclipse.

* Make Gradle compile your `.classpath` and `.project` files
    * Enter `protelis-sandbox/` and run `./gradlew eclipse`
* You need to install the following plugins
    * XText
    * [Protelis](http://hephaestus.apice.unibo.it/protelis-build/protelis-parser/protelis.parser.repository/target/repository/)
* Right click on the project and select: `Configure > Add Xtext Nature`
* Create a new Protelis file `foo.pt` in `src/main/protelis`
* Check syntax completion and highlight

## Useful links
* [Alchemist Javadoc](http://alchemist-doc.surge.sh/)
* [Protelis Javadoc](http://protelis-doc.surge.sh/)
* [Protelis tutorial](https://github.com/AlchemistSimulator/Protelis-Incarnation-tutorial)
