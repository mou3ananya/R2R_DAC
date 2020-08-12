# R-2R Digital-To-Analog Converter
This repository will maintain simulation files and other relevant files of the R-2R DAC block worked on in the VSD Summer Online Internship 2020

*Note: Circuit requires further optimization to improve performance. Design yet to be modified.*

## A Glance at the R-2R DAC IP

The  Design Specifications of the DAC Circuit can be found [here](/Documentation/Specifications.pdf).


## Block Diagram of the R-2R DAC IP

 <p align="center">
  <img width="700" height="450" src="/Images/block.png">
</p>

## Circuit Diagram of the R-2R DAC IP

 <p align="center">
  <img width="800" height="500" src="/Images/circuit.png">
</p>



<img align="left" width="60" height="50" src=/Images/ng_logo.png>

## About Ngspice 
Ngspice is an open source mixed-signal circuit simulator.

### Installing Ngspice

#### For Ubuntu

Open your terminal and type the following to install Ngspice
```
$  sudo apt-get install -y ngspice
```

## Running the Simulation


To enter the Ngspice Shell, open the terminal & type:
```
$ ngspice
```
To simulate a netlist, type:
```
ngspice 1 ->  source <filename>.cir
```

You can exit from the Ngspice Shell by typing:
```
ngspice 1 ->  exit
```
 <p align="center"> or </p>
 
```
ngspice 1 ->  quit
```

## Pre-Layout Simulation

To clone the Repository and download the Netlist files for Simulation, enter the following commands in your terminal.

```
$  sudo apt install -y git
$  git clone https://github.com/sherylcorina/R2R_DAC
$  cd R2R_DAC/Simulation/PreLayout/DAC_v1.1/
```

### Transfer Curve of the R-2R DAC [0-1023]

Run the netlist file using the following command.

```
$  ngspice dac_transfer.cir
```
 <p align="center">
  <img width="800" height="500" src="/Images/dac_transfer.png">
</p>

 <p align="center">
  <img width="800" height="500" src="/Images/dac_transfer_ps.png">
</p>


## Issues | Improvements | Future Work

1.  

## Contributors 

- **Sheryl Serrao** 
- **Kunal Ghosh** 


## Acknowledgments

- Kunal Ghosh, Director, VSD Corp. Pvt. Ltd.
- Philipp Gühring, Software Architect, LibreSilicon Assocation
- Saroj Rout, Associate Professor & Chief Mentor of VLSI Center of Excellence SIT, Bhubaneswar, India
- Santunu Sarangi, Asst. Professor, SIT, Bhubaneswar, India
- Tim Edwards, Senior Vice President of Analog and Design at efabless corporation

## Contact Information

- Sheryl Serrao, Undergraduate Student, Mumbai University sherylcorina@gmail.com
- Kunal Ghosh, Director, VSD Corp. Pvt. Ltd. kunalghosh@gmail.com
- Philipp Gühring, Software Architect, LibreSilicon Assocation pg@futureware.at
