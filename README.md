# OpenXRAM
OpenXRAM is an open-source SRAM(/RRAM/MRAM).. compiler developed by RIOS Lab.

Which could generate high performance SRAM IP with open-source techinology.

We are buliding the architecture of this compiler.

![image](https://user-images.githubusercontent.com/109063674/212647474-19261a5a-8632-4d89-a81d-55edf5e494e2.png)

OpenXRAM will be complete industrial level compilers that consist of various open-source generators to satisfy the requirements of the circuit desgin. Each of the final building block, the physical layout, will be implemented as a stand-alone, densely packed, pitch-matched array. 

With this memory design lib and layout generator,these memory cells(SRAM now, and RRAM/MRAM in the feature) can realize extreme density and performance. In each layout
generator, we added an option which makes the aspect ratio of the physical layout selectable so that the processor or ASIC designers can choose the aspect ratio according to the convenience of the chip level layout.

## Generators of Compiler
OpenXRAM memory compiler is a set of various, parameterized lib generators. These generators are:

• Layout Generator(LEF/GDS)
  
  Generates an array of custom, pitch-matched lef cells and final GDSII file.
  
• Schematic Generator & Netlister(CDL)
  
  Generates a spice or CDL netlist which can be used for both LVS and functional verification.
  
• Function & Timing Model Generators(Lib/V)
  
  Generates behavior simulation, dynamic/static timing analysis and synthesis models.

To customize the configuration of memory macro, designer could setup certain numbers to following four generator parameters:

• Number of words (w)

• Number of bits per word (b)

• Lower address decoder type (y)

• Number of banks (ba).

The valid range of these parameters is specified in :

![image](https://user-images.githubusercontent.com/109063674/212657810-57f95adf-3e58-4e13-a83a-2b8c58382af1.png)


## Design Stage
This project has 6 developing stages. And we would present all SRAM tech to the open-source comunity. 
![image](https://user-images.githubusercontent.com/109063674/212635930-cc9b00ad-45dc-404a-9506-e68b9092bbb2.png)

## Roadmap
![image](https://user-images.githubusercontent.com/109063674/212635997-13877596-63b8-48b2-87b0-e80fa63825a7.png)

Memory Compiler（AI based）Roadmap

## EDA Tool Flow
![image](https://user-images.githubusercontent.com/109063674/212636017-53386803-91be-44c0-9cb3-1798460082cb.png)

EDA Design Flow

## Useful Link

ECE 5745 Tutorial 8: SRAM Generators https://cornell-ece5745.github.io/ece5745-tut8-sram/

Ultra-Low-Power SRAM Design In High Variability Advanced CMOS https://core.ac.uk/download/pdf/4417879.pdf

SRAM MEMORY ARCHITECTURE https://repository.iiitd.edu.in/jspui/bitstream/handle/123456789/579/Purnima%20Singh_2012151.pdf

Skywater-digital-flow SRAM Unit design https://code.stanford.edu/ee272/skywater-digital-flow/-/tree/master/SramUnit/design

Open EDA design flow https://priyanka-raina.github.io/ee372-spring2022/

OpenRAM https://github.com/VLSIDA/OpenRAM

OpenSRAM https://github.com/iamkrvikash/OpenSRAM

