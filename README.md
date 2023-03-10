<h1 align="center">
    <a href="ufg.br"><img src="https://github.com/MilleniumSAT/wiki/blob/main/figures/milleniumlogo.png?raw=true" alt="MILLENIUMSAT" width="30%"></a>
    <br>
    MilleniumSAT (ST-OBSAT-01)
    <br>
</h1>

<h4 align="center">Repositório da documentação técnica e teórica da missão.</h4>

<p align="center">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
    <a href="http://ufg.br/en/team/">
		<img src="https://img.shields.io/badge/spacelab%20members-8-blue?style=for-the-badge">
	</a>
	<a href="#license">
		<img src="https://img.shields.io/badge/open--source-project-lightgray?style=for-the-badge">
	</a>
	<a href="http://www.inpe.br/crn/">
		<img src="https://img.shields.io/badge/partner-inpe--rn-yellow?style=for-the-badge">
	</a>
	<a href="http://ufsc.br">
		<img src="https://img.shields.io/badge/sourced%20by-UFSC-orange?style=for-the-badge">
	</a>
	<a href="https://www.gov.br/aeb/pt-br">
		<img src="https://img.shields.io/badge/sourced%20by-AEB-red?style=for-the-badge">
	</a>
    <a href="https://github.com/spacelab-ufsc/floripasat2-doc/actions">
        <img src="https://img.shields.io/github/workflow/status/spacelab-ufsc/floripasat2-doc/Build%20LaTeX%20document?style=for-the-badge">
    </a>
</p>

<p align="center">
  	<a href="#overview">Overview</a> •
  	<a href="#mission-statement">Statement</a> •
  	<a href="#mission-objectives">Objectives</a> •
  	<a href="#mission-requeriments">Requirements</a> •
  	<a href="#mission-schedule">Schedule</a> •
  	<a href="#development">Development</a> •
  	<a href="#partners">Partners</a> •
  	<a href="#licenses">Licenses</a> •
  	<a href="#notes">Notes</a>
</p>


## Overview

A MilleniumSAT é uma missão desenvolvida com o propósito de estudo da Anomalia Magnética do Atlântico Sul.

A Anomalia Magnética do Atlântico Sul (AMAS) é uma área localizada na região do Oceano Atlântico, próxima à costa do Brasil e da África, onde ocorre uma redução significativa na intensidade do campo magnético terrestre em relação a outras regiões do planeta. Essa anomalia foi descoberta em 1958, durante a missão militar americana "Operation Argus", que tinha como objetivo monitorar explosões nucleares atmosféricas.

A AMAS é um fenômeno que intriga cientistas de todo o mundo, já que não existe uma explicação clara para sua origem. Uma das teorias mais aceitas é que a anomalia é causada pela presença de um grande volume de material líquido na região, como o magma presente em vulcões submarinos. Outra possibilidade é que a AMAS seja uma consequência da dinâmica do núcleo terrestre, que é composto principalmente de ferro e níquel, e que gera o campo magnético do planeta.

A importância da AMAS se deve ao fato de que ela interfere na navegação de aviões e navios, uma vez que o campo magnético é utilizado como referência para a orientação. Além disso, a anomalia tem sido estudada por cientistas que buscam entender melhor o funcionamento do campo magnético terrestre e sua relação com os processos geológicos e geofísicos.

Recentemente, foi descoberto que a AMAS está se expandindo em direção à América do Sul, o que tem gerado preocupação entre os cientistas e autoridades. Acredita-se que essa expansão possa ter implicações em diversos aspectos, como a segurança das redes elétricas e de comunicações, além de impactar a navegação e a aviação na região.

Essa proposta foi trabalhada durante a 1º Olimpíada Brasileira de Satélites, e será efetivamente lançada em um lançamento orbital em meados de dezembro de 2023*.

<p align="center">
    <img width="65%" src="https://github.com/MilleniumSAT/wiki/blob/main/figures/pcb-01.png?raw=true" />
</p>

## Objetivo da missão

1. Coletar dados da magnetosfera a fim de ampliar os estudos em relação à Anomalia Magnética do Atlântico Sul.
2. Validar a utilização de um algoritmo de localização e mapeamento do campo magnético chamado Magnetic SLAM.
3. Validar a utilização do sensor magnético de baixo custo RM3100 para missões em cubesats 1U.
4. Analisar a influência de interferências eletromagnéticas no uso do sensor.
5. Enviar os dados adquridos através do subsistema de telemetria utilizando frequências radio-amadoras.
6. Servir como inspiração para futuras missões originárias do Núcleo de Pesquisas Aeroespaciais da Universidade Federal de Goiás.

## Requisitos da missão

1. Deverá haver disponibilidade de um barramento CAN e USART para comunicação do microcontrolador sampler com o OBC
2. Necessidade de uma alimentação 3.3V e 5V
3. Deverá haver um barramento através de conectores header (PC104)
4. Deverá haver previsão de fornecimento de potencia para (580mW) em atividade
5. Deverá haver disponibilidade um andar inteiro para o payload
6. A comunicação entre o computador de bordo e payload deverá seguir o protocolo desenvolvido
7. A órbita deverá estar entre 500~600km de altitude, preferenciamente
8. A inclinação orbital deverá ser 35º e 60º

## Mission Schedule

| Start [+months]  | Finish [+months] | Activity / Phase                                                                                          |
|------------------|------------------|-----------------------------------------------------------------------------------------------------------|
| T304             | T265             | Acquisition and manufacturing of critical elements and components for the solo platform                   |
| T0               | T0 + 4           | Acquisition and manufacture of elements and components critical to the payload                            |
| T0               | T0 + 9           | Acquisition and manufacturing of critical elements and components for the solo segment                    |
| T0               | T0 + 6           | Compatibility tests between platform and payload in SpaceLab UFSC                                         |
| T0 + 4           | T0 + 10          | Integration of the engineering model in SpaceLab UFSC                                                     |
| T0 + 4           | T0 + 11          | Preparation and suitability of the ground segment                                                         |
| T0 + 8           | T0 + 10          | Verification and validation of the engineering model at SpaceLab UFSC                                     |
| T0 + 8           | T0 + 11          | Verification and validation of the flight model at SpaceLab UFSC                                          |
| T0 + 9           | T0 + 12          | Data collection platforms installation                                                                    |
| T0 + 10          | T0 + 11          | Verification and validation tests of Engineering Model compatibility with EMMN in the INPE / CRN in Natal |
| T0 + 10          | T0 + 11          | Environmental tests at the Integration and Testing Laboratory (LIT / INPE)                                |
| T0 + 11          | T0 + 11          | Flight model acceptance and ground segment review                                                         |
| T0 + 9           | T0 + 12          | Ground segment delivery                                                                                   |
| T0 + 11          | T0 + 12          | Flight model delivery                                                                                     |

> T0 = 23 December 2020

## Development 

The following sections describe the mission subsystems, which placement, positioning and attachement can be seen in the next figure. Also, it is provided a quick review of the development status of each module throught the use of dynamic badges. The profile icons right above the module name is the GitHub contributors of this repository, which might not included all contributors to the project as a whole. Refer to the specific repositories or the website for a complete list.  

<p align="center">
  <img width="65%" src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/exploded-view.png" />
</p>

<br><br>

<a href="https://github.com/spacelab-ufsc/obdh2/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=spacelab-ufsc/obdh2" />
</a>

## OBDH - On-Board Data Handling

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/obdh2/releases">
		<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/spacelab-ufsc/obdh2?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/obdh2/commits/master">
		<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/spacelab-ufsc/obdh2?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/obdh2/issues">
		<img alt="GitHub issues" src="https://img.shields.io/github/issues/spacelab-ufsc/obdh2?style=for-the-badge">
	</a>
</p>

<a href="https://github.com/spacelab-ufsc/obdh2">
<img align="right" width="25%" src="https://github.com/spacelab-ufsc/obdh2/blob/master/doc/user_manual/figures/obdh2-pcb-top.png">
</a>

The SpaceLab OBDH2 (On-Board Data Handling 2.0) is one of the service modules developed for GOLDS-UFSC Cubesat Mission. The OBDH2 is responsible to synchronize actions and the data flow between other modules (ie. EPS, Payloads) and the Earth segment. It packs the generated data into data frames and transmit back to Earth through TTC module, or stores it on a non-volatile memory for later retrieval. Commands sent from Earth segment to the cubesat will be received by the radio transceivers located in the TTC module and redirected to the OBDH2, which takes the appropriate action or forward them to the responsible module. All the OBDH2 project, source and documentation files are available freely on a [GitHub repository](https://github.com/spacelab-ufsc/obdh2) under its respective licenses.

<br><br>

<a href="https://github.com/spacelab-ufsc/ttc2/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=spacelab-ufsc/ttc2" />
</a>

## TTC - Telemetry, Tracking and Telecommand

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in--orbit%20validated-blue?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/ttc2/releases">
		<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/spacelab-ufsc/ttc2?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/ttc2/commits/master">
		<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/spacelab-ufsc/ttc2?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/ttc2/issues">
		<img alt="GitHub issues" src="https://img.shields.io/github/issues/spacelab-ufsc/ttc2?style=for-the-badge">
	</a>
</p>

<a href="https://github.com/spacelab-ufsc/ttc2">
<img align="right" width="25%" src="https://github.com/spacelab-ufsc/ttc2/blob/master/doc/user_manual/figures/ttc2_pcb_top.png">
</a>

The TTC (or TT&C) is the communication module of the CubeSats from SpaceLab. It is responsible to make the communication between the earth (a ground station) and a satellite, and is divided in two sub-modules: Beacon and telemetry. The beacon is a independent sub-module who transmits a periodic signal containing an identification data (ID) of the satellite and some basic telemetry data. The telemetry sub-module is the main communication device. It has a bidirectional data link to receive telecommands from the earth and transmit all the requested data. The telemetry sub-module is controlled by an external device (as example, an OBDH module). All the TTC project, source and documentation files are available freely on a [GitHub repository](https://github.com/spacelab-ufsc/ttc) under its respective licenses.

<br><br>

<a href="https://github.com/spacelab-ufsc/eps2/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=spacelab-ufsc/eps2" />
</a>

## EPS - Electrical and Power System

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/eps2/releases">
		<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/spacelab-ufsc/eps2?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/eps2/commits/master">
		<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/spacelab-ufsc/eps2?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/eps2/issues">
		<img alt="GitHub issues" src="https://img.shields.io/github/issues/spacelab-ufsc/eps2?style=for-the-badge">
	</a>
</p>

<a href="https://github.com/spacelab-ufsc/eps2">
<img align="right" width="25%" src="https://github.com/spacelab-ufsc/eps2/blob/master/doc/figures/eps2-pcb-top.png">
</a>

The EPS2 has been designed to harvest, store and distribute energy for the GOLDS-UFSC CubeSat mission. The energy harvesting system is based on solar energy conversion through 10 solar panels attached to the structure. The EPS is designed to operate the solar panels at their maximum power point. The harvested solar energy is stored in 4 lithium-ion batteries connected in series/parallel. The energy distribution is done by several integrated DC-DC converters. The full EPS system is composed of the solar panels, the EPS PCB, and the Batteries PCB. All the EPS2 project, source and documentation files are available freely on a [GitHub repository](https://github.com/spacelab-ufsc/eps2) under its respective licenses.

<br><br>

<a href="https://github.com/spacelab-ufsc/battery-module-4c/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=spacelab-ufsc/battery-module-4c" />
</a>

## BATC4 - Battery Module 4 cells

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/battery-module-4c/releases">
		<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/spacelab-ufsc/battery-module-4c?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/battery-module-4c/commits/master">
		<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/spacelab-ufsc/battery-module-4c?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/battery-module-4c/issues">
		<img alt="GitHub issues" src="https://img.shields.io/github/issues/spacelab-ufsc/battery-module-4c?style=for-the-badge">
	</a>
</p>

<a href="https://github.com/spacelab-ufsc/battery-module-4c">
<img align="right" width="25%" src="https://github.com/spacelab-ufsc/battery-module-4c/blob/master/images/bat2-pcb-bottom.png">
</a>

The battery module is a separeted board from the EPS in order to accommodate 4 lithium-ion cells. Besides the cells, the board has connectors for interfacing signals and power lines with the EPS module, 2 power resistors to operate as heaters to maintain the cells temperature during eclipse periods, and 4 temperature sensors. The batteries used are the ICR18650-30B lithium-ion cells, which are connected in series and parallel to supply the required voltage and current. Each cell is fixed with 18650 metal holders and between the pairs there is the power resistor attached with a thermal element in the middle. Also, a mechanical mount is placed over the batteries and screwed to the board, providing better stress resistance. All the BATC4 project, source and documentation files are available freely on a [GitHub repository](https://github.com/spacelab-ufsc/battery-module-4c) under its respective licenses.

<br><br>

## Payload EDC - Environmental Data Collector Payload

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-under%20testing-yellow?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/release-v1.1-blue?style=for-the-badge">
	</a>
</p>

<img align="right" width="25%" src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/edc-pcb-top.png">

The Environmental Data Collector (EDC) is a CubeSat-compatible payload that decodes signals from Platform Transmitter Terminals (PTTs) belonging to the Brazilian Environmental Data Collection System and the Argos-2 system. The EDC is composed by an RF Front End and a Processing Unit. The processing unit is based on an SoC FPGA, which configures the external components at system initialization, processes the digital signal from the RF Front End and handles the communication with the On-Board Computer (OBC). 

<br><br>

## Payload X - Redundant OBDH

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/release-v1.3-blue?style=for-the-badge">
	</a>
</p>

<img align="right" width="25%" src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/payload-x-pcb-top.png">

The Payload X was developed to perform an in-orbit validation (IOV) of two new technologies: a novel radiationhardened FPGA and an IP Core for telemetry and telecommand following the ECSS/CCSDS standard. The hardware was designed following the European Space Agency (ESA) space product standards. It has a layered structure that mitigates the effects of radiation and electromagnetic interference on the components signals. The implementation stored in the FPGA includes not only the TC/TM IP core, but also an abstract execution graph, in the form of a state machine, emulating the basic functionalities of an on-board computer (OBC). The communications module handles TC and TM data and it is an interface between the radio transceiver and the emulated OBC. The emulated OBC is based on the ECSS Telemetry & Telecommand Packet Utilization Standard (PUS), and it performs the validation of the routed telecommand received, and the packeting of the telemetry data acquired by the available sensors.

<br><br>

## DaughterBoard HARSH - Radiation Monitor

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-under%20testing-yellow?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/release-v0.1-blue?style=for-the-badge">
	</a>
</p>

<img align="right" width="25%" src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/harsh-pcb-top.png">

The Harsh Environment CubeSat DaughterBoard is the result of a partnership between the Space Technology Research Laboratory (UFSC-Brazil) and the Space Radiation Research Group (LIRMM-France). The module was designed to evaluate different manufacture node SDR SDRAM memories in harsh environments. Also, other experiments are performed to analyse the accumulated dose in the board, which might be used to estimate the dose received in the satellite. The board is compatible with the OBDH DaughterBoard standard.

<br><br>

<a href="https://github.com/spacelab-ufsc/interface-board/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=spacelab-ufsc/interface-board" />
</a>

## IIP - Interstage Interface Panels

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/interface-board/releases">
		<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/spacelab-ufsc/interface-board?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/interface-board/commits/master">
		<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/spacelab-ufsc/interface-board?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/interface-board/issues">
		<img alt="GitHub issues" src="https://img.shields.io/github/issues/spacelab-ufsc/interface-board?style=for-the-badge">
	</a>
</p>

<a href="https://github.com/spacelab-ufsc/interface-board">
<img align="right" width="25%" src="https://github.com/spacelab-ufsc/interface-board/blob/master/doc/figures/iip_fullset.PNG">
</a>

Interstage Interface Panels (IIP) are vertical mounted PCBs designed to give external access to the modules inside of a 2U or 3U CubeSat during final assembly, integration and testing. IIP is composed by 3 different boards, the complete set allows for the nanosatellite to be charged, programed and debugged. All the IIP project, source and documentation files are available freely on a [GitHub repository](https://github.com/spacelab-ufsc/interface-board) under its respective licenses.

<br><br>

<a href="https://github.com/spacelab-ufsc/pc104-adapter/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=spacelab-ufsc/pc104-adapter" />
</a>

## PC104-ADPT - PC-104 Adapter

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/pc104-adapter/releases">
		<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/spacelab-ufsc/pc104-adapter?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/pc104-adapter/commits/master">
		<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/spacelab-ufsc/pc104-adapter?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/pc104-adapter/issues">
		<img alt="GitHub issues" src="https://img.shields.io/github/issues/spacelab-ufsc/pc104-adapter?style=for-the-badge">
	</a>
</p>

<a href="https://github.com/spacelab-ufsc/pc104-adapter">
<img align="right" width="25%" src="https://github.com/spacelab-ufsc/pc104-adapter/blob/master/doc/figures/pc104-adapter.png">
</a>

The PC-104 Adapter is a set of two boards that allow the connection between two separated stacks of PC-104 boards using PicoBlade cables. All the 104 pins of the PC-104 connector are connected through the cables. The Top Board has eight PicoBlade connectors (13 pins version) on the bottom side and a PC-104 connector (female) on the top side. The Bottom Board has eight PicoBlade connectors (13 pins version) on the top side and a PC-104 connector (male) on the bottom side. All the PC104-ADPT project, source and documentation files are available freely on a [GitHub repository](https://github.com/spacelab-ufsc/interface-board) under its respective licenses.

<br><br>

## ACS - Attitude Control System

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in--orbit%20validated-blue?style=for-the-badge">
	</a>
</p>

<img align="right" width="25%" src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/adcs.png">

Our Attitude Control System (ACS) is a passive attitude system, which uses Earth's magnetic field to rotate and stabilize the satellite. The system is composed of one magnet to create a force to align the magnet with the Earth's magnetic field and four hysteresis bars to damp the cube oscillations and stabilize. They are placed in positions to minimize the magnet effect on the bars. As a passive magnetic attitude control system is used, it is possible to stabilize only two axis, and so, the cubesat will still rotate around one of its axis, even after stabilized.

<br><br>

## USIPED - 2U Mechanical Structure

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-under%20testing-yellow?style=for-the-badge">
	</a>
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/purchased%20module-USIPED-lightgray?style=for-the-badge">
	</a>
</p>

<img align="right" width="25%" src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/usiped-2u-structure.jpg">

The USIPED 2-Unit CubeSat structure is developed as a generic, modular satellite structure based upon the CubeSat standard. The modular chassis allows for up to two 1-Unit stack of PCBs, or other modules, to be mounted inside the chassis, using the PC-104 standard and spacers attached to the structure. In addition, there are 4 slots in the middle section, providing space for the interface boards and the ACS. The solar panels and antennas are externally mounted, providing a complete mechanical solution.

<br><br>

## ISIS - Antennas

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in--orbit%20validated-blue?style=for-the-badge">
	</a>
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/purchased%20module-ISIS-lightgray?style=for-the-badge">
	</a>
</p>

<img align="right" width="25%" src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/isis-antenna.png">

The ISISPACE CubeSat Antenna System 1U/3U contains up to four tape spring antennas of up to 55 cm length. The deployment system relies on a thermal knife composed of one wire and two redundant heating elements per tape. RF phasing / BalUn circuitry ties the antennas together in the user-defined configuration. Depending on the configuration, one or two radios in the CubeSat can connect to the antenna system by means of miniature RF connectors. The top face of the antenna system can accommodate a two solar cell solar panel and it can be customized for accommodating sensors or other systems to protrude to the exterior, e.g. camera apertures. The antenna is compatible with any UHF and/or VHF radio system. It can be mounted on all ISIS CubeSat structures and Pumpkin rev C and rev D CubeSat structures. For custom made structures, which adhere to the CubeSat standard mechanical envelope, mounting should also be possible.

<br><br>

## ORBITAL - Solar Panels

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-flight%20ready-green?style=for-the-badge">
	</a>
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/purchased%20module-ORBITAL-lightgray?style=for-the-badge">
	</a>
</p>

<img align="right" width="25%" src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/orbital-solar-panel.png">

The solar panels are manufactures by ORBITAL, a Brazilian company. The panels features protection diodes and high-efficiency solar cells, which are the CESI's CTJ-30 with dimensions 6.9 cm x 3.9 cm (area 26.5 cm2). This cell is qualified for space use by ESA with an efficiency of 29.5% (AM0, BOL). The panels do not include magnetorquers, sensors and others devices.

<br><br>

<a href="https://github.com/spacelab-ufsc/flatsat-platform/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=spacelab-ufsc/flatsat-platform" />
</a>

## FlatSat - FlatSat Test Platform

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/flatsat-platform/releases">
		<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/spacelab-ufsc/flatsat-platform?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/flatsat-platform/commits/master">
		<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/spacelab-ufsc/flatsat-platform?style=for-the-badge">
	</a>
	<a href="https://github.com/spacelab-ufsc/flatsat-platform/issues">
		<img alt="GitHub issues" src="https://img.shields.io/github/issues/spacelab-ufsc/flatsat-platform?style=for-the-badge">
	</a>
</p>

<a href="https://github.com/spacelab-ufsc/flatsat-platform">
<img align="right" width="25%" src="https://github.com/spacelab-ufsc/flatsat-platform/blob/master/doc/figures/flatsat_top_image.PNG">
</a>

The SpaceLab FlatSat Platform is a testbed for cubesat pcb modules. FlatSats enable easier, faster and secure method for testing subsystens indenpently or integrated in a flat design before going to assembly on a cubesat standard. The PCB can support up to 7 modules, all PC104 pins are interligated with each respective counterpart to flexibilize its use, only the particularity connection between modules need to be be taken into account. All the PC104-ADPT project, source and documentation files are available freely on a [GitHub repository](https://github.com/spacelab-ufsc/flatsat-platform) under its respective licenses.

<br><br>

<a href="https://github.com/MilleniumSAT/wiki-decoder/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=MilleniumSAT/wiki-decoder" />
</a>

## SpaceLab Packet Decoder

<p align="left">
	<a href="https://github.com/MilleniumSAT/wiki#versioning">
		<img src="https://img.shields.io/badge/status-in%20development-red?style=for-the-badge">
	</a>
	<a href="https://github.com/MilleniumSAT/wiki-decoder/releases">
		<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/MilleniumSAT/wiki-decoder?style=for-the-badge">
	</a>
	<a href="https://github.com/MilleniumSAT/wiki-decoder/commits/master">
		<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/MilleniumSAT/wiki-decoder?style=for-the-badge">
	</a>
	<a href="https://github.com/MilleniumSAT/wiki-decoder/issues">
		<img alt="GitHub issues" src="https://img.shields.io/github/issues/MilleniumSAT/wiki-decoder?style=for-the-badge">
	</a>
</p>

<a href="https://github.com/MilleniumSAT/wiki-decoder">
<img align="right" width="25%" src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/spacelab-decoder.png">
</a>

SpaceLab Packet Decoder is a software to decode audio records from the satellites of SpaceLab. For now, this software is still under development and are not functional yet.

<br><br>

## Partners

#### Space Technology Research Laboratory (SpaceLab)

<p float="left">
  	<a href="https://spacelab.ufsc.br/">
  		<img src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/spacelab-logo-full-color-rgb-1000px%4072ppi.png" width="37%" />
  	</a>
</p>

#### Federal University of Santa Catarina (UFSC)

<p float="left">
    <a href="https://ufsc.br/">
        <img src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/ufsc-logo.png" width="30%" />
    </a>
</p>

#### National Institute for Space Research - Northeast Regional Center (INPE-RN)

<p float="left">
  	<a href="http://www.inpe.br/crn/">
  		<img src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/inpe-logo.png" width="23%" />
  	</a> 
</p>

#### Brazilian Space Agency (AEB)

<p float="left">
  	<a href="https://www.gov.br/aeb/pt-br">
  		<img src="https://github.com/spacelab-ufsc/golds-ufsc-doc/blob/master/figures/aeb-logo.png" width="27%" />
  	</a>
</p>

## Licenses

The SpaceLab follows a strong open-source approach in order to encourage and promote knowledge. Then, refer to the LICENSE file in the GitHub page for each repository. This mission uses different open-source licenses accordingly to projects needs and restrictions. It is used GNU General Public License v3.0 for firmware sources, CERN Open Hardware License v2.0 for hardware files, and CC BY-SA 4.0 for the documentation. Some third-part files and libraries are subjected to their specific terms and licenses. Please, double check licenses and third-part components used with other licenses, since restrictions might apply.

## Notes

This repository includes the sources of the main documentation. In order to edit/compile/generate, check the following:  

#### Dependencies

* ```latexmk```
* ```texlive-epstopdf```

#### Generating the PDF file

```
make
```
