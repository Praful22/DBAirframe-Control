# Modified-DBAirframe-Control 
Design, Linearize, Trim, and Implementation of Pitch Rate Controller for DeHavilland Beaver Airframe model in SIMULINK.
Credit: https://www.youtube.com/watch?v=FSDB5Gn9hts 


# DeHavilland Beaver with a float landing gear
![aeroplano-659310_1280 (1)](https://github.com/Praful22/Modified-DBAirframe-Control/assets/65821250/197bbc4e-f2ed-4176-a085-b1d2a10f35be)

# Aircraft Components Breakdown
<img width="894" alt="SketchAircraft" src="https://github.com/Praful22/Modified-DBAirframe-Control/blob/main/IMG_5903.jpg">

# Dehavilland Beaver Aircraft Simulink Model
<img width="894" alt="DehavillandModel" src="https://github.com/Praful22/Modified-DBAirframe-Control/assets/65821250/b37fb716-b748-4682-a3e0-890fbcdbf2dd">

# Break Down of DeHavilland Beaver Aircraft Model
The model shown above for Dehavilland aircraft control consists of three major subsystems. They are listed below:
1. Pilot
2. Environment
3. Dehavilland Beaver Airframe (Vehicle-related Parameters and Aircraft Dynamics)


The control inputs to the aircraft are modeled using the Pilot subsystem whereas the environmental effect that an aircraft observes is modeled as the environment subsystem.

# Pilot Subsystem:
Pilot subsystem consists of four Inports which are the four control parameters that the pilot (or autopilot) can vary depending upon necessary situations.

<img width="1426" alt="Screenshot 2023-08-05 at 2 56 44 PM" src="https://github.com/Praful22/Modified-DBAirframe-Control/assets/65821250/c33564a9-a244-43fb-a37c-af8730c1b8c8">

The inports are described below:
1. Aileron: Control surface that extends from about the midpoint of each wing outward toward the tip, and moves in opposite directions to create aerodynamic forces that cause the **airplane to roll.** <img width="1426" alt="Wing Components Drawing" src="https://github.com/Praful22/Modified-DBAirframe-Control/blob/main/IMG_5880.jpg">

2. Elevator: The component of the empennage system which is attached to the back of the horizontal stabilizer and is used to move the nose of the airplane up and down during flight.

3. Rudder: The component of the empennage system which is  attached to the back of the vertical stabilizer and is used to move the airplane's nose left and right during flight.

<img width="1426" alt="Empennage Components" src="https://github.com/Praful22/Modified-DBAirframe-Control/blob/main/IMG_5899.jpg" caption="Empennage System">

4. Throttle :

# Environment Subsystem: 
The environment subsystem consists of major environment parameters that affect the DHV aircraft on the flight. They are shear forces due to air, drag, and wind profiles depending upon the height at which the aircraft is flying.
<img width="1426" alt="Screenshot 2023-08-05 at 2 57 45 PM" src="https://github.com/Praful22/Modified-DBAirframe-Control/assets/65821250/d59bfcf6-ab8a-46c7-b7f6-5197d3c0c518">

1. WGS84 gravity Model: The WGS84 gravity model is derived from the World System Geodesic 84 model which models the earth as an oblate spheroid (see picture below taken from Wikipedia). The model block takes position in geodesic latitude, longitude, and height and outputs the gravitational acceleration.
<img width="800" src="https://github.com/Praful22/Modified-DBAirframe-Control/blob/main/WGS84reference.png" caption="Oblate Spheroid">

2. COESA Atmosphere Model: The COESA Atmosphere Model block is the mathematical representation of the 1976 Committee on Extension to the Standard Atmosphere (COESA) United States standard lower atmospheric(11-12 miles (18-20 km) high at the equator, 5½ miles (9 km) at 50°N and 50°S, and just under four miles (6 km) high at the poles.) values for absolute temperature, pressure, density, and speed of sound for the input geopotential altitude.

3. Wind Models: The wind models need separate and thorough introductions and descriptions so they are broken down into respective models below.

## Wind Models breakdown:

1. Wind Shear Model :
2. Dryden Wind Turbulence Model :
3. Discrete Wind Gust Model :

# DeHavilland Beaver's Dynamics and Parameters Breakdown:
DeHavilland Beaver's Dynamics and Parameters
<img width="1426" alt="Screenshot 2023-08-05 at 3 00 04 PM" src="https://github.com/Praful22/Modified-DBAirframe-Control/assets/65821250/4dfe1d23-cf98-4cbf-8e72-b3ced17885e6">

## Parameter Calculation

## Aircraft Dynamics
<img width="1426" alt="Aircraft Dynamics" src="https://github.com/Praful22/Modified-DBAirframe-Control/blob/main/6DOFEOM.png">
