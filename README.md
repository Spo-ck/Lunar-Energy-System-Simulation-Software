# Lunar Energy System Simulation Software LES3

The Lunar Energy System Simulation Software LES3 has been developed as a modular software for the simulation of space ELectrical Power Systems EPS on the surface of the moon. It is consisting out of sequential models developed as python classes, which allow to simulate space EPS in a much simpler way than standard approaches and employs a great level of details and complexity. A minimum number of required parameters needs to be indicated in the initialization of a simulation python class and all remaining parameters will be loaded from dedicated internal databases. Inidividual system modules can be imported into each other and simulations are carried out automatically once started. The development of individual simulations for different EPS topologies or the wiring known from standard software is not required with this approach. Instead, it is sufficient to import individual models and the simulation will adapt itself.
Irradiance on the lunar surface is simulated based on a kepler orbit simulator and reference frames as direct solar irradiance, earth albedo & infrared irradiance and lunar albedo & infrared irradiance. The simulation of solar cells and batteries is based on the datasheet parameters of all space certifyed solar cells and batteries currently available, that have been integrated into dedicated databases. These are employed by single solar cell and battery models, which are themselves employed in the simulation of solar arrays and battery packs. Into the simulation of solar arrays, also the simulation of solar array tracking and shadowing has been integrated. These system models can in the next step be imported into the simulation of DC/DC-Converters. Eight converter topologies have been implemented, including space standard topologies such as Weinberg and S3R. Different combinations of feedforward-, proportional-, integrative- and differential-control, as well as maximum power point tracking and multi-domain-control algorithms have been implemented into the simulator. The load model is based on a reference circuit and allows to simulate both, static and time-series loads. In addition to this, a Main- BUS-Capacitor class has been implemented. The Main-BUS class allows to simulate a DC Main-BUS consisting out of a flexible combination of different DC/DC converters, a Main-BUS-Capacitor and directly connected loads. In addition to this, the energy grid class alows to simulate multiple interconnected DC Main-BUSes.

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/LES3Topology.png?raw=true)

## Content
1. ![Product Features](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/tree/main#product-features)
2. ![Environmental Model](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/tree/main#environmental-model)
3. ![Lunar Energy System Simulation Software](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/tree/main#lunar-energy-system-simulation-software)
4. ![Contact Details](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/tree/main#contact-details)

## Product Features

➔ Database of 40 space certified solar cells

➔ Database of 29 space certified batteries

➔ Solar cell model including shadowed I(V)-Curve

➔ Multiple different battery cell Models

➔ Different solar array tracking modes

➔ Solar cell thermal model

➔ EQ-Flux solar cell Degradation model integrated

➔ Creme96, AE-/AP-8 radiation models and Chandrayaan data based radiation model integrated

➔ Kepler orbit model

➔ Planck-spectrum for direct solar, earth albedo & infrared and lunar albedo & infrared irradiance

➔ 8 DC/DC-Converter topologies built in, including S3R- and Weinberg Converters

➔ Different control methods built in, including different combinations of FPID-Controllers, MPPT- and (Multi-)
Domain-Control

➔ Time-Series and reference-circuit based load model

➔ Main-BUS-Capacitor model

➔ Main BUS model allows to simulate multiple interconnected DC BUSes with different voltage levels

➔ Regenerative Fuel Cell and Nuclear Reactor models, as well as NASA SPICE will be integrated into a later
version

## Environmental Model

A part of the LES3 software is a simulator for the environmental conditions on the lunar surface. This software has been developed for the authors Master's Thesis, which covers the development of the simulation software, and a global study with focus on the application of photovoltaic generators on the lunar surface

Master's Thesis: [Development of a simulator for the operational conditions of photovoltaic power generators on the lunar surface and implications of environmental conditions to photovoltaic generator design and optimisation](https://www.researchgate.net/publication/377111324_Development_of_a_simulator_for_the_operational_conditions_of_photovoltaic_power_generators_on_the_lunar_surface_and_implications_of_environmental_conditions_to_photovoltaic_generator_design_and_optimi)

### Software Models

#### Geometrical Simulator
![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Geometrical-Simulator.png)

*Geometrical Simulator*

#### Black Body Irradiance Simulator

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Irradiance.png?raw=true)

*Geometrical Simulator*

#### Black Body Irradiance Simulator

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Irradiance.png?raw=true)

*Black Body Irradiance Simulator*

#### Irradiance Simulator

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Irradiance%20Solar%20IR.png?raw=true)

*Solar Irradiance and Earth IR Irradiance*

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Irradiance%20Earth%20ALbedo.png?raw=true)

*Earth Albedo Irradiance*

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Irradiance%20Lunar%20Albedo.png?raw=true)

*Lunar Albedo Irradiance*

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Irradiance%20Lunar%20IR.png?raw=true)

*Lunar IR Irradiance*

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Irradiance-Simulator.png)

*Irradiance Simulator*

#### Particle Radiation and Solar Cell Degradation Simulator

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Radiation%20Model.png)

*Particle Radiation Model*

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Lunar%20Radiation%20Damping%20Field%20Model.png?raw=true)

*Lunar Particle Radiation Damping Model*

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Lunar%20Radiation%20Damping%20Field%20Model%202.png?raw=true)

*Lunar Particle Radiation Damping Model*

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Particle-Radiation-and-Solar-Cell-degradation-Model.png)

*Particle Radiation and Solar Cell Degradation Model*

#### Thermal and Thermal Control System Model

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Thermal-Model-and-Thermal-Control-System-Model.png)

*Thermal Model and Thermal Control System Model*

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Thermal%20Management%20SYSTEM%20MODEL.png?raw=true)

*Thermal Control System Model*

#### Software Structure

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Software-Structure-of-the-Environmental-Simulation-Software.png)

*Software Structure of the Environmental Simulation Software*

### Study with focus on the application of Photovoltaics on the lunar surface

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/assets/53335971/1be65d0d-8e96-4441-91e5-84e968f742f9)

*Lunar Irradiance Sankey*

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Reviewed%20Cases.png?raw=true)

*Reviewed Cases*

#### Solar Irradiance Progression

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Solar%20Irradiance%20Lunar%20Surface.png?raw=true)

*Solar Irradiance Progression*

#### Earth Albedo Irradiance Progression

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Earth%20Albedo%20Irradiance%20Lunar%20Surface.png?raw=true)

*Earth Albedo Irradiance Progression*

#### Solar Elevation Progression

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Solar%20Elevation%20Lunar%20Surface.png?raw=true)

*Solar Elevation Progression*

#### Earth Elevation Progression

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Earth%20Elevation%20Lunar%20Surface.png?raw=true)

*Earth Elevation Progression*

#### Horizontal Irradiance on the Lunar SUrface in the visible spectrum progression

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Horizontal%20Solar%20Irradiance%20Lunar%20Surface.png?raw=true)

*Horizontal Irradiance on the Lunar SUrface in the visible spectrum progression*

#### Temperature Simulation Lunar Surface

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Lunar%20Surface%20Temperature.png?raw=true)

*Temperature Simulation Lunar Surface*

#### Solar Array Mounting and Tracking Systems employing Tracking Systems

##### Solar Incidence Angle Progression

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Solar%20Array%20Mounting%20and%20Tracking.png?raw=true)

*Solar Incidence Angle Progression employing tracking systems*

##### Solar Irradiance Analysis

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Solar%20Array%20Mounting%20and%20Tracking%20Study.png?raw=true)

*Solar Irradiance Analysis*

#### Solar Cell Temperature Progression

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/SOlar%20Array%20Temperature%20SImulation.png?raw=true)

*Solar Cell Temperature Progression*

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/SOlar%20Array%20Temperature%20SImulation%202.png?raw=true)

*Solar Cell Temperature Progression*

##### Temperature Progression employing Thermal Management Systems

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Solar%20Array%20Thermal%20Management.png?raw=true)

*Temperature Progression employing Thermal Management Systems*

##### Thermal Management System Study

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Environmental-Model/Solar%20Array%20Thermal%20Management%20Study.png?raw=true)

*Thermal Management System Study*

#### Solar Cell Degradation Simulation

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/assets/53335971/a6f1f468-623b-4ebc-bc91-2da448a4da62)

*Solar Cell Degradation Simulation*

## Lunar Energy System Simulation Software

The LES3 software is currently a part of my PHD, and therefore I cannot yet make it available for public use.

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/Software%20Overview%20LES3.png)

*Software Structure of the LES3 Software*

## Contact Details

If you have any questions, feel free to contact me.

Mail: jan@zuenkler.eu
