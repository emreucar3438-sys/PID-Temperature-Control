# PID-Temperature-Control
# PID Temperature Control with Disturbance Rejection

This project simulates a simple thermal system controlled by a PID controller.

The goal is to keep the temperature at **50°C** while the system is affected by an external disturbance.

## Features

- PID temperature control
- Proportional, Integral and Derivative terms
- Heater power saturation (0–150 W)
- Disturbance at 100 seconds
- Anti-windup using conditional integration
- Comparison with and without PID

## System

The thermal model is based on:

- Initial temperature: 25°C
- Target temperature: 50°C
- Thermal capacity: 500 J/°C
- Heater power: 150 W
- Simulation time: 500 s

At 100 seconds, the heat loss coefficient changes from **2 to 5 W/°C** to simulate a disturbance.
PID gains were tuned experimentally to achieve fast response while minimizing overshoot.

## Result

The PID controller adjusts the heater power according to the temperature error and helps the system respond to the disturbance.

The actuator is limited to 150 W, so the controller also includes anti-windup to prevent excessive integral accumulation.

## Tools

- MATLAB

## Author

Emre
