# Protelis-Sandbox

A sandbox environment for debugging Protelis code through [Alchemist Simulator](https://github.com/AlchemistSimulator/Alchemist)

## Getting Started

These instructions describe how to set up and run the simulation

### Structure

How the simulation is structured

```
/protelis-sandbox/src/main/
|------> effects/ (add effects to the simulation)
|------> protelis/ (protelis code)
|------> resources/ (maps, ...)
|------> yaml/ (simulation configuration)
```
### Dependencies

Change the `alchemistVersion` in `gradle.properties` to run the simulation with a different Alchemist release

### Modify and run the simulation

To execute the simulation
```
cd protelis-sandbox
./gradlew
```

Modify `simulation` in `gradle.properties` to change the simulation which will be executed. Note that by default simulation effects should have the same name of the simulation.