This document was initially created using the website <https://products.aspose.app/words/conversion/docx-to-md> and subsequently edited for neatness and coherency.

<br/>

# HELICS Integration Survey

## Survey of Commercial and Research Tools with HELICS Integration

<br/>
<br/>

30 June 2023

Georgia Tech Research Institute (GTRI)

Cybersecurity, Information, Protection, and Hardware Evaluation Research (CIPHER)

Embedded Systems Vulnerability Division (ESVD)

Adam King

<br/>
<br/>

# Table of Contents
[Overview](#_toc139022044)

&emsp;&emsp;[Acknowledgements](#_toc139022045)

[Software Inventory](#_toc139022046)

&emsp;&emsp;[Open-Source Integrations and Examples](#_toc139022047)

&emsp;&emsp;&emsp;&emsp;[BEAM (Behavior, Energy, Autonomy, and Mobility)](#_toc139022048)

&emsp;&emsp;&emsp;&emsp;[CYMDIST (CYME Applications for Distribution)](#_toc139022049)

&emsp;&emsp;&emsp;&emsp;[EnergyPlus](#_toc139022050)

&emsp;&emsp;&emsp;&emsp;[GridAPPS-D](#_toc139022051)

&emsp;&emsp;&emsp;&emsp;[GridDyn](#_toc139022052)

&emsp;&emsp;&emsp;&emsp;[GridLAB-D](#_toc139022053)

&emsp;&emsp;&emsp;&emsp;[InterPSS (Power System Simulator)](#_toc139022054)

&emsp;&emsp;&emsp;&emsp;[MATPOWER](#_toc139022055)

&emsp;&emsp;&emsp;&emsp;[ns-3](#_toc139022056)

&emsp;&emsp;&emsp;&emsp;[OMNeT++ (Open Modular Network Testbed in C++)](#_toc139022057)

&emsp;&emsp;&emsp;&emsp;[OpenDSS (Distribution System Simulator)](#_toc139022058)

&emsp;&emsp;&emsp;&emsp;[PFLOW](#_toc139022059)

&emsp;&emsp;&emsp;&emsp;[PSLF (Positive Sequence Load Flow)](#_toc139022060)

&emsp;&emsp;&emsp;&emsp;[PSS/E (Power System Simulator for Engineering)](#_toc139022061)

&emsp;&emsp;&emsp;&emsp;[PMU](#_toc139022062)

&emsp;&emsp;&emsp;&emsp;[PSST (Power System Simulation Toolbox)](#_toc139022063)

&emsp;&emsp;&emsp;&emsp;[PST (Power System Toolbox)](#_toc139022064)

&emsp;&emsp;&emsp;&emsp;[PYPOWER](#_toc139022065)

&emsp;&emsp;&emsp;&emsp;[SAInt (Scenario Analysis Interface)](#_toc139022066)

&emsp;&emsp;&emsp;&emsp;[TESP (Transactive Energy Simulation Platform)](#_toc139022067)

&emsp;&emsp;[Publication of Integrations](#_toc139022068)

&emsp;&emsp;&emsp;&emsp;[ADMS (Advanced Distribution Management Systems)](#_toc139022069)

&emsp;&emsp;&emsp;&emsp;[ANDES](#_toc139022070)

&emsp;&emsp;&emsp;&emsp;[DNP3 (Distributed Network Protocol 3)](#_toc139022071)

&emsp;&emsp;&emsp;&emsp;[FESTIV (Flexible Energy Scheduling Tool for Integrating Variable Generation)](#_toc139022072)

&emsp;&emsp;&emsp;&emsp;[JuMP](#_toc139022073)

&emsp;&emsp;&emsp;&emsp;[NGfast](#_toc139022074)

&emsp;&emsp;&emsp;&emsp;[NGTransient](#_toc139022075)

&emsp;&emsp;&emsp;&emsp;[OCHRE](#_toc139022076)

&emsp;&emsp;&emsp;&emsp;[OMF (Open Modeling Framework)](#_toc139022077)

&emsp;&emsp;&emsp;&emsp;[OPAL-RT](#_toc139022078)

&emsp;&emsp;&emsp;&emsp;[pandapower](#_toc139022079)

&emsp;&emsp;&emsp;&emsp;[PLEXOS](#_toc139022080)

&emsp;&emsp;&emsp;&emsp;[POLARIS](#_toc139022081)

&emsp;&emsp;&emsp;&emsp;[PowerWorld](#_toc139022082)

&emsp;&emsp;&emsp;&emsp;[RTDS (Real-Time Digital Simulator)](#_toc139022083)

&emsp;&emsp;[Absent Integrations](#_toc139022084)

&emsp;&emsp;&emsp;&emsp;[CAPE (PSS/CAPE) (Computer Aided Protection Engineering)](#_toc139022085)

&emsp;&emsp;&emsp;&emsp;[DCAT (Dynamic Contingency Analysis Tool)](#_toc139022086)

&emsp;&emsp;&emsp;&emsp;[GAMS (Generic Algebraic Modeling System)](#_toc139022087)

&emsp;&emsp;&emsp;&emsp;[GasModels.jl](#_toc139022088)

[Software Catalog](#_toc139022089)

&emsp;&emsp;[Contingency Analysis](#_toc139022090)

&emsp;&emsp;[Electricity Distribution](#_toc139022091)

&emsp;&emsp;[Electricity Markets](#_toc139022092)

&emsp;&emsp;[Electricity Transmission](#_toc139022093)

&emsp;&emsp;[Gas Pipeline Modeling](#_toc139022094)

&emsp;&emsp;[Miscellaneous](#_toc139022095)

&emsp;&emsp;[Optimization Packages](#_toc139022096)

&emsp;&emsp;[Real-Time Simulation](#_toc139022097)

&emsp;&emsp;[Telecommunication](#_toc139022098)

&emsp;&emsp;[Transportation](#_toc139022099)

[HELICS Videos](#_toc139022100)

&emsp;&emsp;[Topic Matrix](#_toc139022101)

&emsp;&emsp;[Adaptive VVO with PV](#_toc139022102)

&emsp;&emsp;[Aggregate Protection of Dynamic Composite Load Model](#_toc139022103)

&emsp;&emsp;[Electric Power and Natural Gas Co-Simulation with SAInt](#_toc139022104)

&emsp;&emsp;[Integration with NRECA's Open Modeling Framework](#_toc139022105)

&emsp;&emsp;[Multi-Site Co-Simulation Demo](#_toc139022106)

&emsp;&emsp;[Natural Gas and Electric Power Co-Optimization](#_toc139022107)

&emsp;&emsp;[T+D Co-Simulation Convergence](#_toc139022108)

&emsp;&emsp;[Telecommunications](#_toc139022109)

&emsp;&emsp;[Transactive Communities](#_toc139022110)

&emsp;&emsp;[Transportation Co-Simulation with BEAM and OpenDSS](#_toc139022111)

&emsp;&emsp;[Transportation Co-Simulation with POLARIS and OpenDSS](#_toc139022112)

[Appendix A: Acronyms](#_toc139022113)

<br/>
<br/>

# <a name="_toc139022044"></a>Overview
This document seeks to give specific examples of the Hierarchical Engine for Large-scale Infrastructure Co-Simulation (HELICS) framework with extant real-world industrial or research simulations. Specifically, this document compiles information readily available online through public software repositories, videos, and/or research publications.

<br/>

## <a name="_toc139022045"></a>Acknowledgements
This work was done under the Embedded Systems Vulnerability Division (ESVD) within the Cybersecurity, Information, Protection, and Hardware Evaluation Research (CIPHER) laboratory in the Georgia Tech Research Institute (GTRI). Permission was granted from management within ESVD to make this document freely-available online.

<br/>
<br/>

# <a name="_toc139022046"></a>Software Inventory
This section provides a list of frameworks which, at some level, integrate with HELICS. Detailed information for each framework is broken out in a separate section. Additionally, the below section is partitioned into the following groups:

- Frameworks which have open-source code that either (i) internally integrates with HELICS or (ii) provides examples of integration with HELICS; note this does not mean the framework itself is open-source.
- Frameworks which are publicly documented to be integrated with HELICS but which do not have any open-source code to do so
- Frameworks which are claimed to be integrated with HELICS, but which do not have any publications or open-source code which provide direct evidence

<br/>

## <a name="_toc139022047"></a>Open-Source Integrations and Examples
As mentioned above, this section lists frameworks whose HELICS interfaces/examples are freely available online. Frameworks which are closed-source, paid, and/or proprietary are still listed below if their HELICS integrations are open-source.

### <a name="_toc139022048"></a>BEAM (Behavior, Energy, Autonomy, and Mobility)
### <a name="_toc139022049"></a>CYMDIST (CYME Applications for Distribution)
### <a name="_toc139022050"></a>EnergyPlus
### <a name="_toc139022051"></a>GridAPPS-D
### <a name="_toc139022052"></a>GridDyn
### <a name="_toc139022053"></a>GridLAB-D
### <a name="_toc139022054"></a>InterPSS (Power System Simulator)
### <a name="_toc139022055"></a>MATPOWER
### <a name="_toc139022056"></a>ns-3
### <a name="_toc139022057"></a>OMNeT++ (Open Modular Network Testbed in C++)
### <a name="_toc139022058"></a>OpenDSS (Distribution System Simulator)
### <a name="_toc139022059"></a>PFLOW
### <a name="_toc139022060"></a>PSLF (Positive Sequence Load Flow)
### <a name="_toc139022061"></a>PSS/E (Power System Simulator for Engineering)
### <a name="_toc139022062"></a>PMU
### <a name="_toc139022063"></a>PSST (Power System Simulation Toolbox)
### <a name="_toc139022064"></a>PST (Power System Toolbox)
### <a name="_toc139022065"></a>PYPOWER
### <a name="_toc139022066"></a>SAInt (Scenario Analysis Interface)
### <a name="_toc139022067"></a>TESP (Transactive Energy Simulation Platform)

<br/>
<br/>

## <a name="_toc139022068"></a>Publication of Integrations
This section lists frameworks which have been publicized through videos or research papers that discuss integration with HELICS but which do not have freely-available software that demonstrates this. Note this may be due to restrictions within the relevant organizations which prevent them from publishing source code.

### <a name="_toc139022069"></a>ADMS (Advanced Distribution Management Systems)
### <a name="_toc139022070"></a>ANDES
### <a name="_toc139022071"></a>DNP3 (Distributed Network Protocol 3)
### <a name="_toc139022072"></a>FESTIV (Flexible Energy Scheduling Tool for Integrating Variable Generation) 
### <a name="_toc139022073"></a>JuMP
### <a name="_toc139022074"></a>NGfast
### <a name="_toc139022075"></a>NGTransient
### <a name="_toc139022076"></a>OCHRE
### <a name="_toc139022077"></a>OMF (Open Modeling Framework)
### <a name="_toc139022078"></a>OPAL-RT
### <a name="_toc139022079"></a>pandapower
### <a name="_toc139022080"></a>PLEXOS
### <a name="_toc139022081"></a>POLARIS
### <a name="_toc139022082"></a>PowerWorld
### <a name="_toc139022083"></a>RTDS (Real-Time Digital Simulator)

<br/>
<br/>

## <a name="_toc139022084"></a>Absent Integrations
As mentioned above, this section lists frameworks which claim to have integration with HELICS, but which do not seem to have any freely-available documentation of HELICS integration online. This may be due to non-public conversation between organizations, but this is unknown.

### <a name="_toc139022085"></a>CAPE (PSS/CAPE) (Computer Aided Protection Engineering)
### <a name="_toc139022086"></a>DCAT (Dynamic Contingency Analysis Tool)
### <a name="_toc139022087"></a>GAMS (Generic Algebraic Modeling System)
### <a name="_toc139022088"></a>GasModels.jl

<br/>
<br/>

# <a name="_toc139022089"></a>Software Catalog
This section provides links to various references for each framework. While this catalog is intended to be exhaustive, the data may be inaccurate or incomplete. In general, information for each framework includes:

- the original home or reference of the framework
- the main software repository for the framework (if open-source)
- links to software examples which showcase HELICS integration (if available)
- research publications which mention HELICS integration
- videos uploaded from the main HELICS YouTube account from past showcases

<br/>

## <a name="_toc139022090"></a>Contingency Analysis

CAPE (PSS/CAPE) (Computer Aided Protection Engineering)

- <https://www.siemens.com/global/en/products/energy/grid-software/maintain/grid-resiliency-software/psscape.html>
  - “PSSCAPE (previously known as Electrocon's CAPE software) supports protection engineers from transmission utilities, large distribution utilities, and some generation owners with their entire workflow including detailed protection data collection, electronic setting management, setting calculations and validation. With its extensive library of highly detailed relay models and selection of modular protection tools, engineers can seamlessly manage voluminous and complex network data, uncover potential problems, and examine alternative solutions.”

DCAT (Dynamic Contingency Analysis Tool)

- <https://www.pnnl.gov/copyright/dynamic-contingency-analysis-tool-dcat-evaluating-power-grid-cascading-outage-potential>
  - “The Dynamic Contingency Analysis Tool (DCAT) is an open-platform and publicly available methodology to help develop applications that aim to improve the capabilities of power system planning engineers to assess the impact and likelihood of extreme contingencies and potential cascading events across their systems and interconnections. Outputs from the DCAT will help find mitigation solutions to reduce the risk of cascading outages in technically sound and effective ways.”
- <https://www.pnnl.gov/main/publications/external/technical_reports/PNNL-26197.pdf>
  - *User manual publication which discusses how to use and run DCAT*

<br/>

## <a name="_toc139022091"></a>Electricity Distribution

ADMS (Advanced Distribution Management Systems)

- <https://www.nrel.gov/grid/advanced-distribution-management.html>
  - “The ADMS test bed is an evaluation platform that consists of software simulations of large-scale distribution systems and field equipment integrated through hardware-in-the-loop techniques that realistically represent a power distribution system to a commercial or precommercial ADMS. The ADMS is interfaced to the test bed using industry standard communication protocols so it can be deployed as it would be in a utility environment. The test bed can integrate distribution system hardware in the Energy Systems Integration Facility for hardware-in-the-loop experiments and makes use of the facility’s advanced visualization capabilities, including 3D visualization. The test bed can also integrate simulations of end-use loads in buildings as well as home energy management system controllers with the distribution system simulation using the Hierarchical Engine for Large-scale Infrastructure Co-Simulation (HELICS), an open-source, cyber-physical-energy co-simulation framework for electric power systems.”
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*

CYMDIST (CYME Applications for Distribution)

- <https://www.cyme.com/software/cymdist/>
  - “CYMDIST is the distribution system analysis base package of the CYME software. It bundles all the modeling and analysis tools required to perform the various types of simulations involved in electric distribution system planning. The calculation engines support balanced or unbalanced distribution models that are built with any combination of phases and operated in radial, looped or meshed configurations.”
- [https://github.com/GMLC-TDC/cymepy/](https://github.com/GMLC-TDC/cymepy/tree/master)
  - *Python interface between HELICS and CYMDIST*
- <https://github.com/AadilLatif/HELICS-Examples/tree/coconvergence/co-convergence_helper>
  - *This is the work presented in the “T&D Co-Simulation Convergence” video under “Transmission and Distribution”*
  - *This example uses both CYMDIST and PSS/E, but it references model files which are not included in the repository*
  - *Of note is that, while the code was merged into the main HELICS-Examples repository with the pull request (PR) found at <https://github.com/GMLC-TDC/HELICS-Examples/pull/57> with commit <https://github.com/GMLC-TDC/HELICS-Examples/commit/b206493bd7b9cca02d19d59c24bfefe7467d803b>, the current main branch of HELICS-Examples does not seem to have this code included*

- <https://youtu.be/t5PKCqSyfxw>
  - *This is the video “T+D Co-Simulation Convergence”*
- <https://youtu.be/m4BnoCGIa1I>
  - *This is the video “Multi-Site Co-Simulation Demo”*

EnergyPlus

- <https://energyplus.net/>
  - “EnergyPlus™ is a whole building energy simulation program that engineers, architects, and researchers use to model both energy consumption—for heating, cooling, ventilation, lighting and plug and process loads—and water use in buildings.”
- <https://github.com/NREL/EnergyPlus>
  - *The main repository for the EnergyPlus software*
- [https://github.com/pnnl/tesp/](https://github.com/pnnl/tesp/tree/main)
  - *Example PNNL repository showing how to interface with EnergyPlus, GridLAB-D, ns-3, PSST, PYPOWER* 
- <https://github.com/Yuanliang-Li/PEMT-CoSim>
  - *Example repository showing how to interface with EnergyPlus, GridLAB-D, and PYPOWER*
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*

GridAPPS-D

- <https://www.gridapps-d.org/>
  - “GridAPPS-D is an open-source platform that accelerates development and deployment of portable applications for advanced distribution management and operations.”
- <https://github.com/GRIDAPPSD/gridappsd-docker>
  - *The main repository of the GridAPPS-D software*
  - ***The GRIDAPPSD organization over this repository has several other repositories that contain HELICS integration example***
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*



GridLAB-D

- <https://www.gridlabd.org/>
  - “GridLAB-D is a flexible simulation environment that can be integrated with a variety of third-party data management and analysis tools. The core of GridLAB-D has an advanced algorithm that simultaneously coordinates the state of millions of independent devices, each of which is described by multiple differential equations. The advantages of this algorithm over traditional finite difference-based simulators are: 1) it handles unusual situations much more accurately; 2) it handles widely disparate time scales, ranging from sub-seconds to many years; and 3) it is very easy to integrate with new modules and third-party systems.”
- <https://github.com/gridlab-d/gridlab-d>
  - *The main repository for the GridLAB-D software*
- [https://github.com/GMLC-TDC/HELICS-Tutorial/](https://github.com/GMLC-TDC/HELICS-Tutorial/tree/main)
  - *Example HELICS repository showing how to interface with GridLAB-D, GridDyn, FESTIV, and PSST*
- [https://github.com/nathantgray/HELICS-Examples/gridlabd_helics3](https://github.com/nathantgray/HELICS-Examples/tree/main/gridlabd_helics3)
  - *This is a fork of the main HELICS-Examples repository that demonstrates HELICS integration with GridLAB-D*
- <https://github.com/GMLC-TDC/HELICS-Use-Cases/tree/main/PNNL-TD-Dynamic-Load>
  - *Example HELICS repository showing how to interface with GridLAB-D and InterPSS*
- <https://github.com/GMLC-TDC/HELICS-Use-Cases/tree/main/PNNL-Real-Time-Transactive-Energy>
  - *Example HELICS repository showing how to interface with GridLAB-D and MATPOWER*
- <https://github.com/GMLC-TDC/HELICS-Use-Cases/tree/main/ANL_adaptive_volt_var>
  - *Example HELICS repository showing how to interface with GridLAB-D and PFLOW*
- [https://github.com/pnnl/tesp/](https://github.com/pnnl/tesp/tree/main)
  - *Example PNNL repository showing how to interface with EnergyPlus, GridLAB-D, ns-3, PSST, PYPOWER* 
- <https://github.com/Yuanliang-Li/PEMT-CoSim>
  - *Example repository showing how to interface with EnergyPlus, GridLAB-D, and PYPOWER*
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*
- <https://youtu.be/mesbmRBPKSU>
  - *This is the video “Adaptive VVO with PV”*
- <https://youtu.be/NAfzfojzRlU>
  - *This is the video “Aggregate Protection of Dynamic Composite Load Model”*
- <https://youtu.be/oVt0UEdpV9A>
  - *This is the video “Transactive Communities”*



OCHRE

- <https://www.nrel.gov/grid/ochre.html>
  - “Residential buildings are seeing growth in demand-side technologies; rooftop solar, electric vehicles, and energy storage systems; and smart, energy-efficient heat pumps. Many of these devices are “smart” and equipped with cloud-connected controllers that enable advanced control. OCHRE can simulate new control opportunities at scale and identify potential grid benefits and impacts. OCHRE uses detailed thermal and electrical modeling of residential end uses and devices and integrates with grid simulators and device controllers.”
- <https://www.sciencedirect.com/science/article/pii/S0142061520342095>
  - *Research paper which discusses HELICS integration with OCHRE, OpenDSS, and PLEXOS for testing and evaluation of transactive energy markets*
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*

OMF (Open Modeling Framework)

- <https://www.omf.coop>
  - ***Account necessary to use system***
- <https://github.com/dpinney/omf>
  - “The Open Modeling Framework (OMF) is a set of Python libraries for simulating power systems behavior with an emphasis on cost-benefit analysis of emerging technologies: distributed generation, storage, networked controls, etc.”
  - *This is the main repository for the OMF software*
- <https://youtu.be/71gtYp8e8jE>
  - *This is the video “Integration with NRECA’s Open Modeling Framework”*

OpenDSS (Distribution System Simulator)

- <https://www.epri.com/pages/sa/opendss>
  - “OpenDSS is an electric power distribution system simulator (DSS) designed to support distributed energy resource (DER) grid integration and grid modernization. It enables engineers to perform complex analyses using a flexible, customizable, and easy to use platform intended specifically to meet current and future distribution system challenges and provides a foundation for understanding and integrating new technologies and resources.”
- <https://sourceforge.net/projects/electricdss/>
  - *The main repository for the OpenDSS software*
- <https://github.com/dss-extensions/OpenDSSDirect.py>
  - *Python wrapper for OpenDSS*
- <https://github.com/NREL/PyDSS>
  - *Python interface between HELICS and OpenDSS*
- <https://github.com/GMLC-TDC/HELICS-Use-Cases/tree/main/ANL-TD-Iterative-Pflow>
  - *Example HELICS repository showing how to interface with OpenDSS and PFLOW*
- <https://github.com/GMLC-TDC/pesgm-2019-helics-tutorial/tree/master/notebooks/OpenDSSDirect_PyPower_CoSim>
  - *Example HELICS repository showing how to interface with OpenDSS and PYPOWER*
- <https://www.energy.gov/sites/default/files/2021-07/elt258_meintz_2021_o_5-28_225pm_LR_ML.pdf>
  - *Publication from the National Renewable Energy Laboratory (NREL) which discusses integration of OpenDSS (PyDSS) and BEAM with HELICS*
  - *This seems to correspond to the “Transportation Co-Simulation with BEAM and PyDSS” video under “Transportation”*
- <https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9569771>
  - *Research paper which discusses the creation of a co-simulation framework for distributed energy resource (DER) frequency response using HELICS, ANDES, and OpenDSS*
- <https://www.sciencedirect.com/science/article/pii/S0142061520342095>
  - *Research paper which discusses HELICS integration with OCHRE, OpenDSS, and PLEXOS for testing and evaluation of transactive energy markets*
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*
- <https://youtu.be/i0AHiBtKoE8>
  - *Video from OPAL-RT which discusses HELICS integration with OpenDSS and OPAL-RT*
- <https://youtu.be/rC0D9qEtYHw>
  - *This is the video “Transportation Co-Simulation with BEAM and OpenDSS”*
- <https://youtu.be/Jjqxa7Z40L0>
  - *This is the video “Transportation Co-Simulation with POLARIS and OpenDSS”*
- <https://youtu.be/m4BnoCGIa1I>
  - *This is the video “Multi-Site Co-Simulation Demo”*

<br/>

## <a name="_toc139022092"></a>Electricity Markets

FESTIV (Flexible Energy Scheduling Tool for Integrating Variable Generation)

- <https://www.nrel.gov/grid/festiv-model.html>
  - “FESTIV is a multiple-timescale, interconnected simulation tool that includes security-constrained unit commitment, security-constrained economic dispatch, and automatic generation control sub-models. Each sub-model is connected to subsequent sub-models such that the output of one sub-model serves as the input to the next. FESTIV is completely configurable so that the effects of different operating temporal resolutions and operating strategies can be explored. FESTIV produces not only economic metrics but also reliability metrics. This enables FESTIV to fully investigate the trade-offs in economic benefits, reliability benefits, and incentive structures.”
- <https://github.com/NREL/FESTIV_MODEL>
  - *This is the main repository for the FESTIV software*
- [https://github.com/GMLC-TDC/HELICS-Tutorial/](https://github.com/GMLC-TDC/HELICS-Tutorial/tree/main)
  - *Example HELICS repository showing how to interface with GridLAB-D, GridDyn, FESTIV, and PSST*
  - ***Examples incomplete***
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*

PLEXOS

- <https://www.energyexemplar.com/plexos>
  - “PLEXOS gives you the power to unify all your data streams – in any granularity – into a single, unified energy modeling and forecasting platform. Its powerful simulation engine analyzes zonal and nodal energy models ranging from long-term investment planning to medium-term operational planning and down to short-term, hourly, and intra-hourly market simulations.”
- <https://www.sciencedirect.com/science/article/pii/S0142061520342095>
  - *Research paper which discusses HELICS integration with OCHRE, OpenDSS, and PLEXOS for testing and evaluation of transactive energy markets*



TESP (Transactive Energy Simulation Platform)

- <https://www.pnnl.gov/projects/transactive-systems-program/simulation-platform-tesp>
  - “The Transactive Energy Simulation Platform, or TESP, was established to reduce the software development effort for simulation of new transactive systems and mechanisms and to provide a consistent basis for analysis.”
- <https://github.com/pnnl/tesp>
  - *This is the main repository for the TESP software*
- <https://github.com/pnnl/tesp/tree/main/src/gridlabd>
  - *TESP repository with examples for GridLAB-D*
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*

<br/>

## <a name="_toc139022093"></a>Electricity Transmission

ANDES

- <https://docs.andes.app/en/latest/>
  - “ANDES is an open-source Python library for power system modeling, computation, analysis, and control, serving as the core simulation engine for the CURENT Large scale Testbed (LTB). It supports power flows calculation, transient stability simulation, and small-signal stability analysis for transmission systems. ANDES implements a symbolic-numeric framework for rapid prototyping of differential-algebraic equation-based models. In this framework, a comprehensive library of models is developed, including the full second-generation renewable models.”
- <https://github.com/CURENT/andes/>
  - *The main repository for the ANDES software*
- <https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9518779>
  - *Research paper which discusses impacts of communication delays on automatic generation control using HELICS and ANDES*
- <https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9569771>
  - *Research paper which discusses the creation of a co-simulation framework for distributed energy resource (DER) frequency response using HELICS, ANDES, and OpenDSS*

GridDyn

- <https://software.llnl.gov/news/2016/08/17/griddyn/>
  - “GridDyn is a power system simulator developed at Lawrence Livermore National Laboratory. The name is a concatenation of Grid Dynamics, and as such usually pronounced as ‘Grid Dine’. It was created to meet a research need for exploring coupling between transmission, distribution, and communications system simulations.”
- <https://github.com/LLNL/GridDyn>
  - *The main repository for the GridDyn software*
- [https://github.com/GMLC-TDC/HELICS-Tutorial/](https://github.com/GMLC-TDC/HELICS-Tutorial/tree/main)
  - *Example HELICS repository showing how to interface with GridLAB-D, GridDyn, FESTIV, and PSST*
  - ***Examples incomplete***
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*



InterPSS (Power System Simulator)

- <https://sites.google.com/a/interpss.org/interpss/Home>
  - “InterPSS (Internet technology based Power System Simulator) is a free and open software development project. Simulation is key to enhancing power system design, analysis, diagnosis, and operation. InterPSS fills a need for a simple to use, yet powerful in functionality, modern software technology based software system. InterPSS is distinguished by its open and loosely coupled system architecture. This architecture enables components developed by others to be easily plugged into InterPSS to augment its functionality, and equally important, allows its components to be integrated into other software system.”
- <https://github.com/InterPSS-Project/ipss-common>
  - *The main repository for the InterPSS software*
- <https://github.com/GMLC-TDC/HELICS-Use-Cases/tree/main/PNNL-TD-Dynamic-Load>
  - *Example HELICS repository showing how to interface with GridLAB-D and InterPSS*
- <https://youtu.be/NAfzfojzRlU>
  - *This is the video “Aggregate Protection of Dynamic Composite Load Model”*

MATPOWER

- <https://matpower.org/about/>
  - “MATPOWER is a package of free, open-source Matlab-language M-files for solving steady-state power system simulation and optimization problems, such as:
    - power flow (PF),
    - continuation power flow (CPF),
    - extensible optimal power flow (OPF),
    - unit commitment (UC) and
    - stochastic, secure multi-interval OPF/UC.”
- <https://github.com/MATPOWER/matpower>
  - *The main repository for the MATPOWER software*
- <https://github.com/GMLC-TDC/MATPOWER-wrapper>
  - *MATLAB interface between HELICS and MATPOWER*
- <https://github.com/GMLC-TDC/HELICS-Use-Cases/tree/main/PNNL-Real-Time-Transactive-Energy>
  - *Example HELICS repository showing how to interface with GridLAB-D and MATPOWER*
- <https://github.com/GMLC-TDC/HELICS-Examples/tree/matpower_with_python_example/matlab/matpower-pyload>
  - *This is a non-main branch of the main HELICS-Examples repository that demonstrates HELICS integration with MATPOWER*
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*

- <https://youtu.be/m4BnoCGIa1I>
  - *This is the video “Multi-Site Co-Simulation Demo”*
- <https://youtu.be/3xUWDtRAW6Y>
  - *This is the video “Natural Gas and Electric Power Co-Optimization”*
- <https://youtu.be/oVt0UEdpV9A>
  - *This is the video “Transactive Communities”*

pandapower

- <https://www.pandapower.org/about/>
  - “pandapower builds on the data analysis library pandas and the power system analysis toolbox PYPOWER to create an easy to use network calculation program aimed at automation of analysis and optimization in power systems. What started as a convenience wrapper around PYPOWER has evolved into a stand-alone power systems analysis toolbox with extensive power system model library, an improved power flow solver and many other power systems analysis functions.”
- <https://github.com/e2nIEE/pandapower>
  - *The main repository for the pandapower software*
- <https://dl.acm.org/doi/pdf/10.1145/3573900.3591118>
  - *Research paper which discusses automating integration of existing simulators into HELICS, including pandapower, PowerWorld, Opal-RT, and DNP3*

PFLOW

- <https://github.com/pflow-team/PFLOW>
  - “PFLOW is a steady-state power flow solver that can be used for both transmission and distribution systems. A shared library for PFLOW (for Linux and MacOS) is provided in the lib directory. PFLOW uses numerical routines from the PETSc library that needs to be installed for PFLOW. The code for the transmission-distribution power flow is written in C and it is tested on Ubuntu and MacOS.”
  - *This is the main repository for the PFLOW software*
- <https://github.com/GMLC-TDC/HELICS-Use-Cases/tree/main/ANL_adaptive_volt_var>
  - *Example HELICS repository showing how to interface with GridLAB-D and PFLOW*
- <https://github.com/GMLC-TDC/HELICS-Use-Cases/tree/main/ANL-TD-Iterative-Pflow>
  - *Example HELICS repository showing how to interface with OpenDSS and PFLOW*
- <https://youtu.be/mesbmRBPKSU>
  - *This is the video “Adaptive VVO with PV”*



PowerWorld

- <https://www.powerworld.com/products/simulator/overview>
  - “PowerWorld Simulator is an interactive power system simulation package designed to simulate high voltage power system operation on a time frame ranging from several minutes to several days. The software contains a highly effective power flow analysis package capable of efficiently solving systems of up to 250,000 buses.”
- <https://dl.acm.org/doi/pdf/10.1145/3573900.3591118>
  - *Research paper which discusses automating integration of existing simulators into HELICS, including pandapower, PowerWorld, Opal-RT, and DNP3*

PSLF (Positive Sequence Load Flow)

- <https://www.geenergyconsulting.com/practice-area/software-products/pslf>
  - “Effective power system analysis often requires large-scale simulations and manipulation of large volumes of data. When performing these analyses, efficient algorithms are just as important as the engineering models in which the data is used. [General Electric (GE)] Energy Consulting recognizes these imperatives, and has developed GE PSLF. The algorithms for power-flow and dynamic system analysis in the PSLF suite have been developed to handle large utility-scale systems of up to 125,000 buses. A complete set of tools allows the user to switch smoothly between data visualization, system simulation, and results analysis.”
- [https://github.com/GMLC-TDC/PSLF-wrapper/master](https://github.com/GMLC-TDC/PSLF-wrapper/tree/master)
  - *Python interface between HELICS and PSLF*
  - *The README details how to run the <https://github.com/GMLC-TDC/HELICS-Tutorial/tree/main/tutorials/1-DistributionFederation-ManualStart> example with PSLF via certain modifications*



PSS/E (Power System Simulator for Engineering)

- <https://www.siemens.com/global/en/products/energy/grid-software/planning/pss-software/pss-e.html>
  - “PSSE is used by planning and operations engineers, consultants, universities, and research labs around the world. PSSE allows you to perform a wide variety of analysis functions, including power flow, dynamics, short circuit, contingency analysis, optimal power flow, voltage stability, transient stability simulation, harmonics, time series power flow and much more.”
- <https://github.com/NREL/PyPSSE>
  - *Python interface between HELICS and PSS/E*
- <https://github.com/AadilLatif/HELICS-Examples/tree/coconvergence/co-convergence_helper>
  - *This is the work presented in the “T&D Co-Simulation Convergence” video under “Transmission and Distribution”*
  - *This example uses both CYMDIST and PSS/E, but it references model files which are not included in the repository*
  - *Of note is that, while the code was merged into the main HELICS-Examples repository with the pull request (PR) found at <https://github.com/GMLC-TDC/HELICS-Examples/pull/57> with commit <https://github.com/GMLC-TDC/HELICS-Examples/commit/b206493bd7b9cca02d19d59c24bfefe7467d803b>, the current main branch of HELICS-Examples does not seem to have this code included*
- <https://youtu.be/t5PKCqSyfxw>
  - *This is the video “T+D Co-Simulation Convergence”*

PSST (Power System Simulation Toolbox)

- <https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7747925>
  - *“psst is an open-source Python application for the simulation and analysis of power system models. psst simulates the wholesale market operation by solving a DC Optimal Power Flow (DCOPF), Security Constrained Unit Commitment (SCUC) and a Security Constrained Economic Dispatch (SCED). psst also includes models for the various entities in a power system such as Generator Companies (GenCos), Load Serving Entities (LSEs) and an Independent System Operator (ISO).”*
- <https://github.com/kdheepak/psst>
  - *The main repository for the PSST software*
- [https://github.com/GMLC-TDC/HELICS-Tutorial/](https://github.com/GMLC-TDC/HELICS-Tutorial/tree/main)
  - *Example HELICS repository showing how to interface with GridLAB-D, GridDyn, FESTIV, and PSST*
  - ***Examples incomplete***
- [https://github.com/pnnl/tesp/](https://github.com/pnnl/tesp/tree/main)
  - *Example PNNL repository showing how to interface with EnergyPlus, GridLAB-D, ns-3, PSST, PYPOWER* 



PST (Power System Toolbox)

- [https://web.archive.org/web/20190807140148/https://www.eps.ee.kth.se/personal/vanfretti/pst/Power_System_Toolbox_Webpage/PST.html](https://web.archive.org/web/20190807140148/https:/www.eps.ee.kth.se/personal/vanfretti/pst/Power_System_Toolbox_Webpage/PST.html)
  - “PST consists of a set of coordinated MATLAB m-files which model the power system components necessary for power system power flow and stability studies. The toolbox comes with the m-files, demo examples of how the models can be used, several sets of dynamic data and a user's manuals.”
- <https://sites.ecse.rpi.edu/~chowj/>
  - *This seems to be the only site that gives access to the PST download for the software and the user manual*
- <https://github.com/GMLC-TDC/HELICS-Use-Cases/PNNL-Wide-Area-Control>
  - *Example HELICS repository showing how to interface with ns-3 and Matlab’s PST*

PYPOWER

- <https://github.com/rwl/PYPOWER>
  - *The main repository for the PYPOWER software*
  - “PYPOWER is a power flow and Optimal Power Flow (OPF) solver. It is a port of MATPOWER to the Python programming language.”
- [https://github.com/pnnl/tesp/](https://github.com/pnnl/tesp/tree/main)
  - *Example PNNL repository showing how to interface with EnergyPlus, GridLAB-D, ns-3, PSST, PYPOWER* 
- <https://github.com/Yuanliang-Li/PEMT-CoSim>
  - *Example repository showing how to interface with EnergyPlus, GridLAB-D, and PYPOWER*
- <https://github.com/GMLC-TDC/pesgm-2019-helics-tutorial/tree/master/notebooks/OpenDSSDirect_PyPower_CoSim>
  - *Example HELICS repository showing how to interface with OpenDSS and PYPOWER*

SAInt (Scenario Analysis Interface)

- <https://www.encoord.com/solutions/saint>
  - “The Scenario Analysis Interface for Energy Systems is a software platform designed to model integrated energy networks and markets [for electricity and natural gas].”
- <https://www.encoord.com/resources/case-studies/helics>
  - *Page from encoord briefly discussing HELICS integration with SAInt*
- <https://github.com/NREL/SAInt_HELICS_interface>
  - *C# interface between HELICS and SAInt*
- <https://youtu.be/m4BnoCGIa1I>
  - *This is the video “Multi-Site Co-Simulation Demo”*
- <https://youtu.be/TcgfFrp9BXQ>
  - *This is the video “Electric Power and Natural Gas Co-Simulation with SAInt”*

<br/>

## <a name="_toc139022094"></a>Gas Pipeline Modeling

GasModels.jl

- <https://lanl-ansi.github.io/GasModels.jl/latest/>
  - “GasModels.jl is a Julia/JuMP package for Gas Network Optimization. It provides utilities for parsing and modifying network data, and is designed to enable computational evaluation of emerging gas network formulations and algorithms in a common platform. It includes support for steady-state and transient formulations.”
- <https://github.com/lanl-ansi/GasModels.jl>
  - *The main repository for the GasModels.jl software*

NGfast

- <https://www.anl.gov/argonne-scientific-publications/pub/58954>
  - “Argonne designed NGfast (written in C Sharp language) to be used as both an impact analysis tool and an information retrieval tool. When used as an impact analysis tool, given the name of the affected pipeline, the location of the break, and the month the event occurred, it provides:
    - A quantitative estimate (tabular) of the impacts to downstream markets
    - A graphic overview of impacts, and, thus, insights into possible restoration strategy options
    - Options to implement mitigating measures
    - An estimate of the net impact after application of mitigation measures (e.g., load shed, states affected, electric megawatts lost”
- <https://www.energy.gov/sites/default/files/2023-02/North%20American%20Energy%20Resiliency%20Model%20Program.pdf>
  - *Research publication discussing integrating various simulations via HELICS to reduce extreme energy infrastructure risk at a national scale*



NGTransient

- <https://f000.backblazeb2.com/file/Imgix-Resilience/2020/10/D4_S2T3_Infrastructure-TED-Talks.pdf>
  - “NGTransient: A Hydraulic Pipeline and Optimal Control Model for Simulating Pipeline Disruptions and Impacts on Electric Power Generation”
  - “Understanding and maintaining operational resilience in interstate natural gas transmission pipelines is crucial to maintaining gas delivery to operators of gas-fired electric generators. Transmission pipelines are subject to physical and regulatory constraints, along with financial constraints and obligations to customers. Gas pressures and flows at delivery points must be maintained at the required conditions of the plant to ensure continuous operation of electric generators. We present the NGTransient hydraulic pipeline model to estimate the impacts of gas pipeline disruptions on power generation using a model of dynamic flow and pressure.”
- <https://youtu.be/3xUWDtRAW6Y>
  - *This is the video “Natural Gas and Electric Power Co-Optimization”*
- <https://youtu.be/m4BnoCGIa1I>
  - *This is the video “Multi-Site Co-Simulation Demo”*

<br/>

## <a name="_toc139022095"></a>Miscellaneous

PMU

- <https://standards.ieee.org/ieee/C37.118.1/4902/>
  - “Synchronized phasor (synchrophasor) measurements for power systems are presented. This standard defines synchrophasors, frequency, and rate of change of frequency (ROCOF) measurement under all operating conditions. It specifies methods for evaluating these measurements and requirements for compliance with the standard under both steady-state and dynamic conditions. Time tag and synchronization requirements are included. Performance requirements are confirmed with a reference model, provided in detail. This document defines a phasor measurement unit (PMU), which can be a stand-alone physical unit or a functional unit within another physical unit. This standard does not specify hardware, software, or a method for computing phasors, frequency, or ROCOF.”
- <https://github.com/GMLC-TDC/HELICS-PMU>
  - *C++ interface between HELICS and PMU*

<br/>

## <a name="_toc139022096"></a>Optimization Packages

GAMS (Generic Algebraic Modeling System)

- <https://www.gams.com/products/gams/gams-language/>
  - “GAMS is a high level modeling system for mathematical programming and optimization. It consists of a language compiler and a range of associated solvers. The GAMS modeling language allows modelers to quickly translate real world optimization problems into computer code. The gams language compiler then translates this code into a format the solvers can understand and solve. This architecture provides great flexibility, by allowing changing the solvers used without changing the model formulation.”

JuMP

- <https://jump.dev/>
  - “JuMP is a modeling language and collection of supporting packages for mathematical optimization in Julia. JuMP makes it easy to formulate and solve a range of problem classes, including linear programs, integer programs, conic programs, semidefinite programs, and constrained nonlinear programs. You can use it to route school buses, schedule trains, plan power grid expansion, or even optimize milk output.”
- <https://youtu.be/3xUWDtRAW6Y>
  - *This is the video “Natural Gas and Electric Power Co-Optimization”*

<br/>

## <a name="_toc139022097"></a>Real-Time Simulation

OPAL-RT

- <https://www.opal-rt.com/>
  - “OPAL-RT is the world leader in the development of PC/FPGA-based real-time simulators, Hardware-in-the-Loop (HIL) testing equipment and Rapid Control Prototyping (RCP) systems to design, test and optimize control and protection systems used in power grids, power electronics, motor drives, automotive, trains, aircraft and various industries, as well as R&D centers and universities.”
- <https://www.opal-rt.com/power-systems-overview/>
  - “OPAL-RT’s power systems product line simulates everything from fast electromagnetic phenomenon to the transient stability of large power systems, all while enabling power systems engineers and scientists to innovate or optimize security, efficiency and performance and protection for the generation, transmission and distribution of power grids.”
- <https://dl.acm.org/doi/pdf/10.1145/3573900.3591118>
  - *Research paper which discusses automating integration of existing simulators into HELICS, including pandapower, PowerWorld, Opal-RT, and DNP3*
- <https://youtu.be/i0AHiBtKoE8>
  - *Video from OPAL-RT which discusses HELICS integration with OpenDSS and OPAL-RT*
- <https://youtu.be/j0LP0qKivyM>
  - *This is the video “Telecommunications”*

RTDS (Real-Time Digital Simulator)

- <https://www.rtds.com/about-rtds-technologies/>
  - “The RTDS Simulator allowed utilities, manufacturers, and research and educational institutions to test multiple devices in a closed loop with the simulated network while easily adjusting network parameters, contingency scenarios, and device settings for the first time.”
- <https://youtu.be/j0LP0qKivyM>
  - *This is the video “Telecommunications”*

<br/>

## <a name="_toc139022098"></a>Telecommunication

DNP3

- <https://www.dnp.org/About/Overview-of-DNP3-Protocol>
  - “The development of DNP3 was a comprehensive effort to achieve open, standards-based Interoperability between substation computers, RTUs, IEDs (Intelligent Electronic Devices) and master stations (except inter-master station communications) for the electric utility industry.”
- <https://standards.ieee.org/ieee/1815/5414/>
  - *IEEE standard of DNP3*
- <https://github.com/dnp3/opendnp3>
  - *C++ implementation of DNP3*
- <https://github.com/ChargePoint/pydnp3>
  - *Python wrapper for the C++ implementation of DNP3*
- <https://github.com/VOLTTRON/dnp3-python>
  - *Redesign of the PyDNP3 Python wrapper*
- <https://dl.acm.org/doi/pdf/10.1145/3573900.3591118>
  - *Research paper which discusses automating integration of existing simulators into HELICS, including pandapower, PowerWorld, Opal-RT, and DNP3*

ns-3

- <https://www.nsnam.org/>
  - “ns-3 is a discrete-event network simulator for Internet systems, targeted primarily for research and educational use. ns-3 is free, open-source software, licensed under the GNU GPLv2 license, and maintained by a worldwide community.”
- <https://gitlab.com/nsnam/ns-3-dev>
  - *The main repository for the ns-3 software*
- <https://github.com/GMLC-TDC/helics-ns3>
  - *C++ interface between HELICS and ns-3*
- [https://github.com/GMLC-TDC/HELICS-Use-Cases/PNNL-Wide-Area-Control](https://github.com/GMLC-TDC/HELICS-Use-Cases/tree/main/PNNL-Wide-Area-Control)
  - *Example HELICS repository showing how to interface with ns-3 and Matlab’s PST*
  - <https://gmlc-tdc.github.io/HELICS-Use-Cases/PNNL-Wide-Area-Control/index.html>
- [https://github.com/pnnl/tesp/](https://github.com/pnnl/tesp/tree/main)
  - *Example PNNL repository showing how to interface with EnergyPlus, GridLAB-D, ns-3, PSST, PYPOWER* 
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*
- <https://youtu.be/j0LP0qKivyM>
  - *This is the video “Telecommunications”*

OMNeT++ (Open Modular Network Testbed in C++)

- <https://omnetpp.org/>
  - “OMNeT++ is an extensible, modular, component-based C++ simulation library and framework, primarily for building network simulators.”
- <https://github.com/omnetpp/omnetpp>
  - *The main repository for the OMNET++ software*
- <https://github.com/GMLC-TDC/helics-omnetpp>
  - *C++ interfafce between HELICS and OMNeT++*
- [https://github.com/pnnl/tesp/](https://github.com/pnnl/tesp/tree/main)
  - *Example PNNL repository showing how to interface with EnergyPlus, GridLAB-D, ns-3, PSST, PYPOWER* 
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*

<br/>

## <a name="_toc139022099"></a>Transportation

BEAM (Behavior, Energy, Autonomy, and Mobility)

- <https://transportation.lbl.gov/beam>
  - “BEAM is an open-source, modular software framework that enables efficient, scalable simulation of regional transportation systems. It allows transportation planners and service providers to simulate traveler behavior and technology deployment to understand congestion, energy, and emission implications of novel mobility technologies and services from individual scale to entire transportation systems.”
- <https://github.com/LBNL-UCB-STI/beam>
  - *This is the main repository for the BEAM software*
  - ***This repository provides examples of HELICS integration with BEAM***
- <https://www.energy.gov/sites/default/files/2021-07/elt258_meintz_2021_o_5-28_225pm_LR_ML.pdf>
  - *Publication from the National Renewable Energy Laboratory (NREL) which discusses integration of OpenDSS (PyDSS) and BEAM with HELICS*
  - *This seems to correspond to the “Transportation Co-Simulation with BEAM and PyDSS” video under “Transportation”*
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*
- <https://youtu.be/rC0D9qEtYHw>
  - *This is the video “Transportation Co-Simulation with BEAM and OpenDSS”*



POLARIS

- <https://vms.taps.anl.gov/tools/polaris/>
  - “Developed by the Argonne National Laboratory Vehicle & Systems Mobility Group (VMS), POLARIS was originally created for the U.S. Department of Transportation (DOT) Federal Highway Administration (FHWA) to analyze transportation system management strategies involving emerging vehicle and information technologies. It has evolved into a high-performance, computationally efficient tool that implements advanced travel and freight demand modeling, dynamic traffic assignment, and transportation simulation into an integrated modeling platform.”
- <https://git-out.gss.anl.gov/polaris/code/polaris-linux>
  - *This is the main repository for the POLARIS software*
  - ***This is only accessible with an Argonne National Laboratory (ANL) account***
- <https://www.osti.gov/servlets/purl/1843579>
  - *Publication that briefly discusses using HELICS with GridLAB-D, OpenDSS, ns-3, MATPOWER, FMI, BEAM, POLARIS, FESTIV, GridDyn, OCHRE, ADMS, GridAPPS-D, EnergyPlus, OMNeT++, TESP*
- <https://youtu.be/Jjqxa7Z40L0>
  - *This is the video “Transportation Co-Simulation with POLARIS and OpenDSS”*

<br/>
<br/>

# <a name="_toc139022100"></a>HELICS Videos
The following videos are from the official HELICS YouTube channel found at <https://www.youtube.com/@tdc-helics9643/videos>. Not all videos from the YouTube channel are covered, as only those videos which detail how HELICS integrates with existing simulations and tools (as opposed to the innerworkings of HELICS) are listed.

<br/>

## <a name="_toc139022101"></a>Topic Matrix

||Electricity Distribution|Electricity Markets|Electricity Transmission|Gas Pipeline Modeling|Optimization Packages|Real-Time Simulation|Telecommunication|Transportation|
| :- | :- | :- | :- | :- | :- | :- | :- | :- |
|[Adaptive VVO with PV](https://youtu.be/mesbmRBPKSU)|X||X||||||
|[Aggregate Protection of Dynamic Composite Load Model](https://youtu.be/NAfzfojzRlU)|X||X||||||
|[Electric Power and Natural Gas Co-Simulation with SAInt](https://youtu.be/TcgfFrp9BXQ)||X|X|X|||||
|[Integration with NRECA's Open Modeling Framework](https://youtu.be/71gtYp8e8jE)|X|X|||||||
|[Multi-Site Co-Simulation Demo](https://youtu.be/m4BnoCGIa1I)|X||X|X|||||
|[Natural Gas and Electric Power Co-Optimization](https://youtu.be/3xUWDtRAW6Y)|||X|X|X||||
|[T+D Co-Simulation Convergence](https://youtu.be/t5PKCqSyfxw)|X||X||||||
|[Telecommunications](https://youtu.be/j0LP0qKivyM)|X||X|||X|X||
|[Transactive Communities](https://youtu.be/oVt0UEdpV9A)||X|X||||||
|[Transportation Co-Simulation with BEAM and OpenDSS](https://youtu.be/rC0D9qEtYHw)|X|||||||X|
|[Transportation Co-Simulation with POLARIS and OpenDSS](https://youtu.be/Jjqxa7Z40L0)|X|||||||X|

<br/>

## <a name="_toc139022102"></a>Adaptive VVO with PV
- <https://youtu.be/mesbmRBPKSU>
- *GridLAB-D, PFLOW*
- “Improving understanding of the interactions between transmission and distribution system through co-simulation”
- “Assessing the voltage regulation functions of smart inverter in regulating the transmission system PCC voltage”
- “[A]ssess the effectiveness of adaptive Volt-VAR control settings in regulating the transmission system voltage when the system load is high”

<br/>

## <a name="_toc139022103"></a>Aggregate Protection of Dynamic Composite Load Model
- <https://youtu.be/NAfzfojzRlU>
- *GridLAB-D, InterPSS*
- “This use case is to provide detailed individual load responses (including the protection actions) to faults in the transmission system to derive the aggregate protection models and evaluate the performance of composite load model CMPLDWG”

<br/>

## <a name="_toc139022104"></a>Electric Power and Natural Gas Co-Simulation with SAInt
- <https://youtu.be/TcgfFrp9BXQ>
- *SAInt*
- “Electric systems can adapt in real-time, but gas network response time depends on topology and conditions”
- “Advanced use case explores implications for the power system if that [historical] flexibility from the gas network had not been available”

<br/>

## <a name="_toc139022105"></a>Integration with NRECA's Open Modeling Framework
- <https://youtu.be/71gtYp8e8jE>
- *GridLAB-D, OMF*
- “Simulate islanded operation of a microgrid”
- “Simulate transient frequency response”
- “Simulate loss of generation”
- “Implement frequency drop based load shedding algorithm”

<br/>

## <a name="_toc139022106"></a>Multi-Site Co-Simulation Demo
- <https://youtu.be/m4BnoCGIa1I>
- *CYMDIST, MATPOWER, NGTransient, OpenDSS, SAInt*
- *Interoperation of various disparate natural gas, transmission, and distribution simulations at different timescales*

<br/>

## <a name="_toc139022107"></a>Natural Gas and Electric Power Co-Optimization
- <https://youtu.be/3xUWDtRAW6Y>
- *MATPOWER, NGTransient*
- “Ability to combine domain specific models, across different languages”
- “If the combined problem is infeasible then it means there exists no feasible solution à one need not worry if the infeasibility is an edge case resulting from how the models were combined”

<br/>

## <a name="_toc139022108"></a>T+D Co-Simulation Convergence
- <https://youtu.be/t5PKCqSyfxw>
- *CYMDIST, OpenDSS, PSS/E*
- “Implementation allows user to run loosely-coupled vs tightly coupled simulations”
- “Allows to enable/disable the co-convergence helper federate”
- “Allows users to scale to more federates easily”

<br/>

## <a name="_toc139022109"></a>Telecommunications
- <https://youtu.be/j0LP0qKivyM>
- *ns-3, OPAL-RT, RTDS*
- “Perform real-time co-simulation of transmission, distribution, and communication using HELICS platform”
- “Perform real-time/HITL simulations by initiating a fault in the transmission system and study the impacts on a distribution system”

<br/>

## <a name="_toc139022110"></a>Transactive Communities
- <https://youtu.be/oVt0UEdpV9A>
- *GridLAB-D, MATPOWER, TESP*
- “Distributed optimal dispatch of price-responsive load and generation”
- “Implementation of both day-ahead and real-time retail energy markets”
- “Implementation of methods to handle communication-system imperfections”

<br/>

## <a name="_toc139022111"></a>Transportation Co-Simulation with BEAM and OpenDSS
- <https://youtu.be/rC0D9qEtYHw>
- *BEAM, OpenDSS*
- *Large-scale San Francisco Bay area system for co-simulation of distribution and electric vehicle charging to schedule charging rates and explore how charger location affects distribution system*

<br/>

## <a name="_toc139022112"></a>Transportation Co-Simulation with POLARIS and OpenDSS
- <https://youtu.be/Jjqxa7Z40L0>
- *OpenDSS, POLARIS*
- “Incorporating EV behavior in grid analysis through co-simulation”
- “Assessing impacts of EVs on distribution system operation”
- “Evaluating mitigation strategies”
- “Making energy policy decisions”

<br/>
<br/>

<a name="_toc138755340"></a>
# <a name="_toc139022113"></a>Appendix A: Acronyms

|Acronym||Meaning|
| :- | :- | :- |
|ADMS||Advanced Distribution Management Systems|
|ANL||Argonne National Laboratory|
|API||Application Programming Interface|
|BEAM||Behavior, Energy, Autonomy, and Mobility|
|BTM||Behind-The-Meter|
|CAPE||Computer Aided Protection Engineering|
|CIPHER||Cybersecurity, Information, Protection, and Hardware Evaluation Research|
|CYMDIST||CYME Applications for Distribution|
|DCAT||Dynamic Contingency Analysis Tool|
|DER||Distributed Energy Resource|
|DERMS||Distributed Energy Resource Management System|
|DSS||Distribution System Simulator|
|ESVD||Embedded Systems Vulnerability Division|
|EV||Electric Vehicle|
|FESTIV||Flexible Energy Scheduling Tool for Integrating Variable Generation|
|GAMS||Generic Algebraic Modeling System|
|GE||General Electric|
|GTRI||Georgia Tech Research Institute|
|HITL||Hardware-In-The-Loop|
|LTB||Large-Scale Testbed|
|NRECA||National Rural Electric Cooperative Association|
|NREL||National Renewable Energy Laboratory|
|OMF||Open Modeling Framework|
|OMNeT++||Open Modular Network Testbed in C++|
|OPF||Optimal Power Flow|
|PMU||Phasor Measurement Unit|
|PR||Pull Request|
|PSLF||Positive Sequence Load Flow|
|PSS||Power System Simulator|
|PSS/E||Power System Simulator for Engineering *(Siemens)*|
|PSST||Power System Simulation Toolbox *(NREL)*|
|PST||Power System Toolbox *(MATLAB)*|
|PyDSS||Python DSS|
|RTDS||Real-Time Digital Simulator|
|SAInt||Scenario Analysis Interface|
|SPMC||Site Power Management Controller|
|T&D||Transmission and Distribution|
|TESP||Transactive Energy Simulation Platform|
