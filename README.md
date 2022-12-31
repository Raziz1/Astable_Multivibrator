# Astable_Multivibrator 🚨
An astable multivibrator circuit designed in Altium Designer

To design the circuit I used the following online guide for an [astable multivibrator circuit](https://www.youtube.com/watch?v=8-BwTmkiMdA&list=PLakVZ0BpR4sJ6X_1DzXHXROfP__xrr5UG&ab_channel=TheEngineeringMindset)

## Introduction
An Astable Multivibrator (Also known as the flip-flop circuit) is a circuit that continuously oscillates between two states. Using transistors, capacitors, and LEDs we can build a circuit to demonstrates its function. 

## Requirements 🗒️
* The transistor needs approximately 0.7V at the base pin to turn on
* Since we are using a 3V supply we will need to use an LED with a low forward voltage (Red & Yellow)
* The arrangmenet of LEDs will be in parallel so that they all have an equal voltage drop 
* I will place a resistor in series with the LED to protect the LED from burning out
* Our targe current for each LED will be 10mA (In parallel that is a total of 50mA) so we will need a 24 ohm resistor 
* I will be using an NPN transistor for this application

## Capacitor Charge Time ⏳
In this circuit the capacitor charge time determines how quickly the LED oscillates. We can adjust how quickly the capacitor charges by adding a resistor in series. The resistor limits the amount of current that enters and leaves the capacitor. The RC time constant describes how quickly a capacitor charges to 63.2% of it's applied DC voltage. The RC time constant is described by the following formula in a simple RC circuit:
* Time constant (Seconds) = Resistance (Ohms) * Capacity (Farads)

Rather than doing math to determine a desired time constant we can fiddle with some values to see the outcomes of the circuits

### OrCad PSPice 
Using OrCad PSPice to simulate the circuit below we can alter the values of the resistor and capacitor and see how it affects the time constant

<p> 
    <img src="https://github.com/Raziz1/Astable_Multivibrator/blob/main/assets/astable_schematic-1.png? raw=true" >
</p> 

### 10 uF voltage response
![image](https://user-images.githubusercontent.com/73625971/209918624-abe01d37-ddb3-4fa4-9b29-4c6e90a2f784.png)

### 100 uF voltage response
![image](https://user-images.githubusercontent.com/73625971/209918794-080cdb8e-b53d-4b29-b3a3-4873efc768ff.png)

### 5 Kohm voltage response
![image](https://user-images.githubusercontent.com/73625971/209919322-2ec8d4ef-e8a1-49ee-9898-866a037290d9.png)

### 22 Kohm voltage response
![image](https://user-images.githubusercontent.com/73625971/209918794-080cdb8e-b53d-4b29-b3a3-4873efc768ff.png)


## Parts
View the BOM to see the parts used for this project

## PCB Layout
The routes for this porject were generated using the autoroute feature. This is not ideal as it can result in a variety of design rule errors. It also does not give you the chance to layout the routes yourself

## Output Files
The following output files were included

* Bill of Materials
* Gerber
* NC Drill
* Pick-and-place
* Board Stackup
* Drill Drawing/Guides
* Schematic Prints
* PCB prints

## 3D View
<img width="441" alt="image" src="https://user-images.githubusercontent.com/73625971/210120348-289c9fdd-42e6-4ce6-92a7-0e84b9af5df6.png">

