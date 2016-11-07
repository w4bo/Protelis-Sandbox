# Protelis-Sandbox
A sandbox environment for debugging Protelis code through Alchemist simulator
## Getting Started

These instructions describe how to set up and run the simulation.

### Structure

How the simulation should be structured.

```
/protelis-sandbox/
|------> effects/ (add effects to the simulation)
|------> protelis/ (protelis code)
|------> resources/ (maps, ...)
|------> yaml/ (simulation configuration)
```
### Dependencies

This project only depends on [Alchemist Simulator](https://github.com/AlchemistSimulator/Alchemist). Change `alchemistVersion` in `gradle.properties` to choose the Alchemist release to run the simulation.

### Modify and run the simulation

To execute the simulation enter `protelis-sandbox/` and run
```
./gradlew
```
To change the simulation to be executed modify `simulation` in `gradle.properties`. Note that by default effects should have the same name of the simulation.