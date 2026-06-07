# EQ-Simulator-Release

# EQ Simulator V1

EQ Simulator V1 is a lightweight 2.5D equipment simulator for PLC logic testing before commissioning.

I built this tool as an automation engineer to solve a practical problem that happens frequently in real PLC projects:  
the machine is not ready yet, but the PLC logic still needs to be tested.

This simulator is not intended to replace professional 3D simulation platforms.  
Instead, it focuses on simple and practical PLC logic verification.

## Main Purpose

- Test PLC logic before the real machine is ready
- Simulate sensors, conveyors, cylinders, units, product flow, and basic equipment behavior
- Reduce debugging pressure during commissioning
- Help PLC engineers verify sequences, interlocks, and timing conditions earlier

## Key Feature: Parent-Child Structure

One of the strongest features of EQ Simulator is the parent-child object structure.

Objects can be assigned to parent units, allowing multiple objects to move and behave as one piece of equipment.

For example:

- A conveyor can be attached to a servo-driven unit
- Sensors can be attached to moving equipment
- Cylinders, conveyors, and sensors can be combined into a custom machine
- Turn conveyors, transfer units, and other compound mechanisms can be built from simple objects

Each object is simple, but the parent-child structure makes it possible to create many different equipment combinations.

## Supported Simulation Objects

- Units
- Sensors
- Lamps
- Switches
- Numeric input and display objects
- Conveyors
- Dog conveyors
- Bowl feeders
- Pipes
- Cylinders
- Hydraulic power units
- Heaters
- Temperature sensors
- Product flow objects

## PLC Communication

EQ Simulator is being developed with the following PLC platforms in mind:

- Allen-Bradley / Rockwell Logix PLCs using libplctag
- Mitsubishi PLCs using MX Component

## Script Support

Virtual units can be controlled using:

- ST-style scripts
- C# scripts

This allows users to create custom motion or behavior that cannot be expressed with simple object settings alone.

## Logging and Analysis

EQ Simulator includes basic analysis tools such as:

- Runtime logs
- Time charts
- Trend graphs
- Automatic timing analysis

These tools are intended to help verify PLC sequence timing and signal behavior.

## Trial Version

The trial version provides full functionality for 30 days.

This application is currently provided as a Windows executable.  
Please scan the downloaded file before running it if needed.

A release package can be downloaded from the Releases section of this repository.

## Notes

This tool was originally created for my own PLC projects and for a specific project team.  
It is not a polished commercial-grade simulator, but it has been useful in real PLC development and commissioning preparation.

Feedback from PLC engineers is welcome.
