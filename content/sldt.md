---
title: Semantic Layer and Digital Twin
sidebar: true # or false to display the sidebar
sidebarlogo: fresh-white-alt # From (static/images/logo/)
include_footer: true # or false to display the footer
---

### Digital Twin
The Digital Twin represents an essential key technology of our age. It connects the physical world with the digital world and acts as an enabler of our Catena-X network. Our open source solution is based on a standardized programming interface of the [Industrial Digital Twin Association (IDTA)](https://industrialdigitaltwin.org) and its [Asset Administration Shell](https://www.plattform-i40.de/IP/Redaktion/DE/Downloads/Publikation/Details_of_the_Asset_Administration_Shell_Part1_V3.html).
The Digital Twin Registry provides a central source of information ("phone book"): all digital twins and their submodels, which contain various aspects of relevant information and services within the data ecosystem, are registered here. In addition to registering new digital twins, they can also be found and viewed at this point along with their submodels.  Digital twins are relevant both for data providers, who supply the agreed data in the agreed form and make it discoverable via the registry, and for data or service users, who can offer value-added services based on this data and find out which providers exist via the registry. The agreed content can be viewed and clearly linked in the Semantic Hub.

### Digital Twin Registry
The Digital Twin Registry is a logical and architectural component of Tractus-X. it is a reference implementations of the SLDT Registry. Its source code can be found [here](https://github.com/eclipse-tractusx/sldt-digital-twin-registry).

### Semantic Hub
Semantic models are used to structure data. As a concept, they make it possible to give fundamental meaning to data and their relationships. In the context of data modeling and data organization, they realize the simple development of applications as well as the maintenance of data consistency.
In Catena-X, semantic data models are provided in a suitable publication system, the so-called Semantic Hub. For data or service providers, the Semantic Hub provides a basis for the use and reuse of semantic models. For this reason, the publication of a semantic data model takes place under the specification of a version. This promotes transparency as well as control over all semantic models and their release status.

The Semantic Hub is a logical and architectural component of Tractus-X. It is a reference implementation of the SLDT Semantic Hub. Its source code can be found [here](https://github.com/eclipse-tractusx/sldt-semantic-hub).
