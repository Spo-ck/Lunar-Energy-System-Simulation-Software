# Lunar Energy System Simulation Software

The Lunar Energy Simulator LES has been developed as a modular software consisting out of sequential models developed as python classes. It allows to simulate space electrical power systems in a much simpler way than standard approaches and employs a great level of details. A minimum number of required parameters needs to be indicated in the initialization of a simulation python class and all remaining parameters will be loaded from dedicated internal databases. Inidividual system modules can be imported into each other and simulations are carried out automatically once started. The development of individual simulations for different EPS topologies or the wiring known from standard software is not required with this approach. Instead, it is sufficient to import individual models and the simulation will adapt itself.
Irradiance on the lunar surface is simulated based on a kepler orbit simulator and reference frames as direct solar irradiance, earth albedo & infrared irradiance and lunar albedo & infrared irradiance. The simulation of solar cells and batteries is based on the datasheet parameters of all space certifyed solar cells and batteries currently available, that have been integrated into dedicated databases. These are employed by single solar cell and battery models, which are themselves employed in the simulation of solar arrays and battery packs. Into the simulation of solar arrays, also the simulation of solar array tracking and shadowing has been integrated. These system models can in the next step be imported into the simulation of DC/DC-Converters. Eight converter topologies have been implemented, including space standard topologies such as Weinberg and S3R. Different combinations of feedforward-, proportional-, integrative- and differential-control, as well as maximum power point tracking and multi-domain-control algorithms have been implemented into the simulator. The load model is based on a reference circuit and allows to simulate both, static and time-series loads. In addition to this, a Main- BUS-Capacitor class has been implemented. The Main-BUS class allows to simulate a DC Main-BUS consisting out of a flexible combination of different DC/DC converters, a Main-BUS-Capacitor and directly connected loads. In addition to this, the energy grid class alows to simulate multiple interconnected DC Main-BUSes.

![image](https://github.com/Spo-ck/Lunar-Energy-System-Simulation-Software/blob/main/Visualization/LES3Topology.png?raw=true)

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
