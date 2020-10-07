# Project of a thermistor based constant temperature anemometer

This repository contains files related to a constant temperature anemometer that uses a self heated NTC thermistor as a sensing element.


## Thermal anemometer

An anemometer is a device that measures fluid speed, in particular air. A thermal anemometer uses heat transfer from a heated element to estimate the velocity of the fluid. There are several ways to build a thermal anemometer but the most common is the use of a self heated resistor whose resistance varies with temperature.

As a side note, a few years ago, José Pucci Caly, a professor at Mackenzie University in São Paulo/Brazil developed with a couple of students a very simple anemometer: the external temperature of the bulb from an incandescent light bulb was calibrated against wind speed. It worked. How well? I don't remember...

There are several ways that a self heated resistor can be used as the two mosto common aproaches are:

 * Constant temperature
 * Constant current

In this project we use the constant temperature approach.

## CTA - Constant temperature anemometer

The basic idea behind the constant temperature anemometer (CTA) is that an electric current passing through a resistor will heat the resistor. The temperature of the resistor is the result of the heat transfer to the fluid flowing around it.

Now suppose that for a given fluid velocity the temperature of the resistor is Tw. If the velocity then increases a tiny bit, Tw should drop a little bit. This drop in temperature corresponds to a change in resistance (when the resistance depends on the temperature). This change in resistance can be picked up and the current flowing through the resistor is changed accordingly.


![Basic feedback circuit](figures/cta-feedback.svg)



