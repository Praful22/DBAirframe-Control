# Modified-DBAirframe-Control
Design, Linearize, Trim, and Implementation of Pitch Rate Controller for DeHavilland Beaver Airframe model in SIMULINK.
Credit: https://www.youtube.com/watch?v=FSDB5Gn9hts 

# Design Object
Model a control scheme to control an inherently unstable airplane using Pitch Rate Controller.

# DeHavilland Beaver with a float landing gear
![aeroplano-659310_1280 (1)](https://github.com/Praful22/Modified-DBAirframe-Control/assets/65821250/197bbc4e-f2ed-4176-a085-b1d2a10f35be)

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

The Inports are described below:
1. Aileron : 
2. Elevator :
=======
# Pilot Subsytem:
Pilot subsystem consists of four inports which are the four control parameters that pilot (or autopilot) can vary depending upon necesarry situations.
The inports are described below:
1. Aileron: Control surface that extends from about the midpoint of each wing outward toward the tip, and move in opposite directions to create aerodynamic forces that cause the airplane to roll.
 <imge width="1426" alt="Wing Components Drawing" src="https://github.com/Praful22/Modified-DBAirframe-Control/blob/main/IMG_5880.jpg"> 
2. Elevator : 
3. Rudder :
4. Throttle :

# Environment Subsystem: 
The environment subsystem consists of major environment parameters that affects the DHV aircraft on flight. They are shear force due to air, drag, and wind profile depending upon height of the aircraft.
<img width="1426" alt="Screenshot 2023-08-05 at 2 57 45 PM" src="https://github.com/Praful22/Modified-DBAirframe-Control/assets/65821250/d59bfcf6-ab8a-46c7-b7f6-5197d3c0c518">

1. WGS84 gravity Model
2. COESA Atmosphere Model
3. Wind Models 

## Wind Models breakdown:

1. Wind Shear Model :
2. Dryden Wind Turbulence Model :
3. Discrete Wind Gust Model :

# DeHavilland Beaver Airframe Breakdown:
The Airframe of DeHavilland Beaver 
<img width="1426" alt="Screenshot 2023-08-05 at 3 00 04 PM" src="https://github.com/Praful22/Modified-DBAirframe-Control/assets/65821250/4dfe1d23-cf98-4cbf-8e72-b3ced17885e6">

## Parameter Calculation
## Aircraft Dynamics
