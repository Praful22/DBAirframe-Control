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
3. Dehavilland Beaver Aircraft

The control inputs to the aircraft is modeled using the Pilot subsystem whereas the environmental effect that an aircraft observes is modeled as the environment subsystem.

# Pilot Subsytem:
Pilot subsystem consists of four inports which are the four control parameters that pilot (or autopilot) can vary depending upon necesarry situations.
The inports are described below:
1. Aileron : 
2. Elevator :
3. Rudder :
4. Throttle :

# Environment Subsystem:
1. WGS84 gravity Model
2. COESA Atmosphere Model
3. Wind Models 
## Wind Models breakdown 

# DeHavilland Beaver Airframe: