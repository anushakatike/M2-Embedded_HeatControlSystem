## Heat Control System 

### Theory

The heat control system is basically used to control the temperature of a car seat. When a user or driver of the car gets seated on a car, the button sensor gets activated. After that, the user gets access to turn on the heater. The temperature sensor keeps monitoring the temperature and sends the analog value to the microcontroller. The microcontroller processes the analog input of the temperature sensor and outputs a temperature value through serial communication. All the activities of the control system are done on a microcontroller called Atmega328.

### Simulation

The functionality of the heat control system is coded in embedded c and the working is demonstrated using simuation in a software called SimulIDE.
Below shows two images where in the 1st image shows the status of the simulation when the system is OFF and the second image shows the status of the system when it is ON. 

#### ON
![Simulation_ON](https://user-images.githubusercontent.com/94188453/144363288-7432f6fd-cdad-4b18-9e3b-5961ef50b140.png)
)

#### OFF
![Simulation_OFF](https://user-images.githubusercontent.com/94188453/144363135-e74f0003-c24e-4d0f-a940-f055b25e0c84.png)
)

#### Outputs

|Circuit|RAM Table|
|:--:|:--:|
|![Circuit](https://user-images.githubusercontent.com/94188453/144363857-28b48024-e503-4b40-ac4d-0b23f9221890.gif)|![RAM_table](https://user-images.githubusercontent.com/94188453/144364012-3ed4a662-7932-410e-8ea6-4d8238b8913f.gif)|
|CRO|Serial Monitor|
|![Oscilloscope](https://user-images.githubusercontent.com/94188453/144364522-371428f2-8bb3-4c49-974d-f35da31d211d.gif)|![Serial_Monitor](https://user-images.githubusercontent.com/94188453/144364647-c76829ec-9896-4149-b9fb-9c784dc77e67.gif)|


### Functionality 

* When the two switches are closed, the first LED glows indicating the actuation of the system and the heater.
* Next the analog input from the temperature sensor is received and digitized.
* The digitized temperature input is visualized using Pulse Width Modulation.
* The corresponding temperature values based on the digitized temperature input is transmitted by the UART protocol. Here the data is displayed on the serial monitor.




### CI and Code Quality

|Build|Cppcheck|Codacy|
|:--:|:--:|:--:|
|[![Compile-Linux](https://github.com/hemanthasapu/embedded_systems_project_256889/actions/workflows/Compile.yml/badge.svg)](https://github.com/hemanthasapu/embedded_systems_project_256889/actions/workflows/Compile.yml)|[![Cppcheck](https://github.com/hemanthasapu/embedded_systems_project_256889/actions/workflows/CodeQuality.yml/badge.svg)](https://github.com/hemanthasapu/embedded_systems_project_256889/actions/workflows/CodeQuality.yml)|[![Codacy Badge](https://app.codacy.com/project/badge/Grade/bf425986b42541fd92f2459de6359d9b)](https://www.codacy.com/gh/hemanthasapu/embedded_systems_project_256889/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=hemanthasapu/embedded_systems_project_256889&amp;utm_campaign=Badge_Grade)|
