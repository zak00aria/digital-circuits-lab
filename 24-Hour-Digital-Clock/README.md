# 24-Hour Digital Clock

A 24-hour digital clock built and simulated using [CircuitVerse](https://circuitverse.org).

The clock uses two-digit counters to represent the hours, minutes, and seconds. Each pair of digits is implemented as a BCD counter built using JK flip-flops.

The seconds counter increments once per second. When it reaches `59`, it resets to `00` and generates a carry signal for the minutes counter. The minutes counter behaves in the same way. When the hours counter reaches `23`, the next clock pulse resets the time to `00:00:00`.

## Preview

![24-hour digital clock demonstration](./24-hour-digital-clock.gif)

## Circuit Simulation

The circuit was designed and simulated in CircuitVerse. You can view how it was built and try the clock using the link below:

[Open the 24-hour digital clock simulation](https://circuitverse.org/users/25835/projects/clock-24-hours)
