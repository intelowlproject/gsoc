# Google Summer of Code 2024
List of project ideas for contributors applying to the Google Summer of Code program in 2024.

## Timeline/milestones
Please always refer to the [official timeline](https://developers.google.com/open-source/gsoc/timeline).
  
## Application Process
Please always refer to the [main page of this repository](https://github.com/intelowlproject/gsoc/blob/main/README.md#gsoc-application-process)

## Project Ideas
You can also propose your own.


### 1. New Documentation Site for IntelOwl and friends
<b>Mentors</b>: Matteo Lodi, Daniele Rosetti

<b>Project URL</b>: [All IntelOwl Organization Projects](https://github.com/intelowlproject) are impacted

<b>Project hours</b>: 175

<b>Skills required</b>: Python (Django) and willingness to explore and adapt to new frameworks and open source projects

<b>Difficulty</b>: Low

<b>Description</b>:

Right now we are not satisfied of how we manage our documentation and how we make it available.

The project aims to create a new repository dedicated to the documentation, move all the documentation of all our projects there and build a new documentation site by leveraging Github Pages and MkDocs.

More information in this [Github Issue](https://github.com/intelowlproject/IntelOwl/issues/2043)

The candidate would have the chance to try some popular tools and to solve a big common problem that a lot of other Open Source projects have.
The ideal candidate is proactive in reading documentation of new tools and excited in trying them to solve our problem.


### 2. Scanners: a new plugin type for IntelOwl
<b>Mentors</b>: Matteo Lodi, Daniele Rosetti, Simone Berni

<b>Project URL</b>: [IntelOwl](https://github.com/intelowlproject/IntelOwl)

<b>Project hours</b>: 175

<b>Skills required</b>: Docker, Python (Django), JavaScript (React.js), Object-Oriented Programming

<b>Difficulty</b>: Medium

<b>Description</b>:

Right now there are many possible types of [plugins](https://intelowl.readthedocs.io/en/latest/Usage.html#plugins) in IntelOwl.

This project aims to add a new plugin type to the already existing ones in IntelOwl:
* The **"Scanner"** type would be a subtype of the “[Analyzers](https://intelowl.readthedocs.io/en/latest/Usage.html#analyzers)” ones with special configuration. In that way, IntelOwl could be used not only for classic data enrichment with external services but as either a vulnerability scanner or a scraper too. Refer to the [Github Issue for more details](https://github.com/intelowlproject/IntelOwl/issues/1393)

Like we have similarly done with other GSoC projects in the past that added new plugin types, we expect the contributor to add the most important new scanners (like [this](https://github.com/intelowlproject/IntelOwl/issues/1021)) to IntelOwl once he finishes building the framework to provide a base of tools which can be used by the users.

The candidate would have the chance to work through all the application stack (backend and frontend).
The ideal candidate for this project is someone who is familiar with how IntelOwl works and its core concepts.


### 3. New Analyzers for IntelOwl
<b>Mentors</b>: Matteo Lodi, Daniele Rosetti, Simone Berni

<b>Project URL</b>: [IntelOwl](https://github.com/intelowlproject/IntelOwl)

<b>Project hours</b>: 175

<b>Skills required</b>: Docker, Python (Django), Object-Oriented Programming

<b>Difficulty</b>: Low

<b>Description</b>:

Right now we have a lot of [Analyzers](https://intelowl.readthedocs.io/en/latest/Usage.html#analyzers) implemented in IntelOwl.

But they are not enough! They are the core part of the application so we want to add even more of them!!!! :)

This project aims to increment the number of available Analyzers. We have about [50 different Analyzers that has been requested by the community members in Github](https://github.com/intelowlproject/IntelOwl/issues?q=is%3Aissue+is%3Aopen+label%3Anew_analyzer+) and are still not implemented. We obviously do not ask to implement all of them but a reasonable amount of them based on the available time and the efforts required for each of them.

Adding a new Analyzer to the framework is one of the easiest things that can be done in this project. Once you get used to it, adding more of them is even easier!

The ideal candidate for this project is someone who understand how IntelOwl's framework works and already tried to implement an Analyzer.

