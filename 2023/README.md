# Google Summer of Code 2023
List of project ideas for contributors applying to the Google Summer of Code program in 2023.

## Timeline/milestones
Please always refer to the [official timeline](https://developers.google.com/open-source/gsoc/timeline).
  
## Application Process
Please always refer to the [main page of this repository](https://github.com/intelowlproject/gsoc/blob/main/README.md#gsoc-application-process)

## Project Ideas
You can also propose your own.

### 1. Ingestors and Scanners: new plugins types for IntelOwl
<b>Mentors</b>: Matteo Lodi, Daniele Rosetti, Simone Berni

<b>Project URL</b>: [IntelOwl](https://github.com/intelowlproject/IntelOwl)

<b>Project hours</b>: 175

<b>Skills required</b>: Docker, Python (Django), JavaScript (React.js), Object-Oriented Programming

<b>Difficulty</b>: Medium

<b>Description</b>:

Right now there are 3 possible types of [plugins](https://intelowl.readthedocs.io/en/latest/Usage.html#plugins) in IntelOwl: “Analyzers”, “Connectors” and “Playbooks”.

This project aims to add 2 new plugin types to the already existing ones in IntelOwl:
* The [“Scanner”](https://github.com/intelowlproject/IntelOwl/issues/1393) type would be a subtype of the “analyzers” ones with special configuration. In that way, IntelOwl could be used not only for classic data enrichment with external services but as either a vulnerability scanner or a scraper too.
* The [“Ingestor”](https://github.com/intelowlproject/IntelOwl/issues/1397) type would be a completely new type of plugin which would work as an input for IntelOwl. In that way, IntelOwl could retrieve observables and files to analyze from an external service.

Like we have similarly done with other GSoC projects in the past that added new plugin types, we expect the contributor to add the most important new scanners/ingestors (like [this](https://github.com/intelowlproject/IntelOwl/issues/1021)) to IntelOwl once he finishes building the framework to provide a base of tools which can be used by the users.

The candidate would have the chance to touch the core parts of the application. Because of this, the ideal candidate for this project is someone who is familiar with how the Plugins Framework works and understands completely how the application leverages it.

### 2. Investigations framework for IntelOwl!
<b>Mentors</b>: Matteo Lodi, Daniele Rosetti, Simone Berni

<b>Project URL</b>: [IntelOwl](https://github.com/intelowlproject/IntelOwl)

<b>Project hours</b>: 175

<b>Skills required</b>: Docker, Python (Django), JavaScript (React.js), Object-Oriented Programming

<b>Difficulty</b>: Hard

<b>Description</b>:

Last GSoC we implemented the [“Playbook”](https://www.honeynet.org/2022/10/06/gsoc-2022-project-summary-creating-playbooks-for-intelowl/) plugin type. Playbooks are designed to be easy to share sequence of running Analyzers/Connectors on a particular kind of observable.
Those are the base to the creation of a new, and more complex framework of analysis that we could call “Investigations framework”. In a nutshell, Investigations are built on top of Playbooks and are thought to be customizable workflows of them. Some discussions [here](https://github.com/intelowlproject/IntelOwl/issues/680) and [here](https://github.com/intelowlproject/IntelOwl/discussions/968) could clarify the intention.

This candidate would have the chance to create a complete new framework from scratch, based on the already existing IntelOwl’s features. Because of this, the ideal candidate for this project is someone who knows very well how the overall application works. This project is highly experimental so a strong critical spirit and adaptability are required.

### 3. Authentication and maintenance of IntelOwl!
<b>Mentors</b>: Matteo Lodi, Daniele Rosetti, Simone Berni

<b>Project URL</b>: [IntelOwl](https://github.com/intelowlproject/IntelOwl), [pyintelowl](https://github.com/intelowlproject/pyintelowl), [GreedyBear](https://github.com/intelowlproject/GreedyBear) and [IntelOwl site](https://github.com/intelowlproject/intelowlproject.github.io)

<b>Project hours</b>: 175

<b>Skills required</b>: Docker, Python (Django), JavaScript (React.js), Object-Oriented Programming

<b>Difficulty</b>: Low/Medium

<b>Description</b>:

This project focuses on adding common features available in classic web applications regarding the management of the authentication and sessions.
[Password reset/change](https://github.com/intelowlproject/IntelOwl/issues/1285) and [2FA](https://github.com/intelowlproject/IntelOwl/issues/1286) are some examples. Others can be proposed by the candidate.

To make the project more complete, we would like the contributor to also take charge of several little stagnant issues in the most important projects (IntelOwl, pyintelowl and GreedyBear) and to solve them, like a classic maintainer would do. During the last year a lot of possible new analyzers and GUI adjustments have been proposed: those are a perfect example of an issue to be solved.

The candidate would have the chance to touch several different parts of the application. Because of this, the ideal candidate for this project is someone who is strongly familiar with IntelOwl codebase.


### 4. Login monitoring and alerting project
<b>Mentors</b>: Federico Foschini

<b>Project URL</b>: [PcapMonkey](https://github.com/certego/PcapMonkey) but a new repo will be created for this project.

<b>Project hours</b>: 175

<b>Skills required</b>: Docker, Python (Django), Javascript, Object-Oriented Programming

<b>Difficulty</b>: Medium

<b>Description</b>:
This new project is a full feature system that lets user ingest login data from various sources(IE: ssh, nginx, azure, etc.) and through a number of correlation rules it generates alerts when a suspicious login is seen. At the moment the project implements all the basic features like user and alerts visualization, a simple dashboard and correlation rules.

During the GSoC period the candidate should work on the following items:

* Settings and configuration page: this feature will allow fine tuning and configuration of the platform
* Alert outputs: implement mail, slack and other integration to allow alerts to be forwarded to other systems
* New log source types: test the project on logs from new sources and write the documentation to allow easy configuration of these sources
* Improve dashboards by showing additional data

The candidate will work on every part of the application, the code base is not very complex but a good knowledge of Django and some javascript for the web interface is strongly recommended.


### 5. More Quark Scripts for CWE Detections!
<b>Mentors</b>: YuShaing Dang, ShengFeng Lu, KunYu Chen

<b>Project URL</b>: [Quark Engine](https://github.com/quark-engine/quark-engine)

<b>Project hours</b>: 175

<b>Skills required</b>: Python, Object-Oriented Programming

<b>Difficulty</b>: Low/Medium

<b>Description</b>:

Last year, Quark Engine shifted its goal from malware detection to vulnerability digging. The project has proposed Quark scripts to detect CWEs (Common Weakness Enumeration). We now have scripts to detect [15 CWEs](https://github.com/quark-engine/quark-engine#cwe-showcases) on Android binaries. And we’d like to grow this number. 

The candidate is required to have clear and critical thinking. Fully understand the definition of the CWEs and develop the detection logic of the CWEs with the Quark Script APIs. 

The candidate needs to understand a little about the codebase of Quark Engine since we may need to develop new APIs for the other CWEs.

### 6. Make the better versality of Quark Scripts!
<b>Mentors</b>: YuShaing Dang, ShengFeng Lu, KunYu Chen

<b>Project URL</b>: [Quark Engine](https://github.com/quark-engine/quark-engine)

<b>Project hours</b>: 175

<b>Skills required</b>: Python, Object-Oriented Programming

<b>Difficulty</b>: Low/Medium

<b>Description</b>:

Last year, Quark Engine shifted its goal from malware detection to vulnerability digging. The project has proposed Quark scripts to detect CWEs (Common Weakness Enumeration). We now have scripts to detect [15 CWEs](https://github.com/quark-engine/quark-engine#cwe-showcases) on Android binaries. However, there is more than just one way to detect a particular CWE. 

So, the candidate is required to have clear and critical thinking. Fully understand the definition of the CWEs and develop new detection logic of the CWEs. Making the better versatility of the scripts. 

The candidate needs to understand a little about the codebase of Quark Engine since we may need to develop new APIs for the other CWEs.

### Generic Important Note
Please note: if the potential contributor would like to invest more time, he can propose a 350 hours project composed of 2 of the 3 proposed projects requirements together!
