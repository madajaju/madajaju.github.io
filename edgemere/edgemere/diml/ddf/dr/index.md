---
layout: default
title: Package Data Repository
permalink: package--edgemere-diml-ddf-dr
---
# Data Repository

Data Repository is a package that contains...



## Use Cases



![UseCase Diagram](./usecases.svg)

## Users


![User Interaction](./userinteraction.svg)

## Interface
The subsystem has a REST, CLI, WebSocket, and Web interface. Use Cases and Scenarios can use any or all
of the interfaces to perform the work that needs to be completed. The following  diagram shows how
users interact with the system.

![Scenario Mappings Diagram](./scenariomapping.svg)



## Logical Artifacts
The Data Model for the  Data Repository shows how the different objects and classes of object interact
and their structure.

![Sub Package Diagram](./subpackage.svg)

### Sub Packages



![Logical Diagram](./logical.svg)

### Classes



## Activities and Flows
The Data Repository subsystem provides the following activities and flows.

### Messages Handled
| Message | Action | Description |
|---|---|---|

|    |    |    |

### Messages Sent

TBD

## Deployment Architecture

This subsystem is deployed using micro-services as shown in the diagram below. The 'micro' module is
used to implement the micro-services in the system.
The subsystem also has an CLI, REST and Web Interface exposed through a sailajs application. The sailsjs
application will interface with the micro-services and can monitor and drive work-flows through the mesh of
micro-services.

![Deployment Image](./deployment.svg)

## Physical Architecture

The Data Repository subsystem is is physically laid out on a hybrid cloud infrastructure. Each microservice is shown
how they connect to each other. All of the micro-services communicate to each other and the main app through a
REST interface. A CLI, REST or Web interface for the app is how other subsystems or actors interact. Requests are
forwarded to micro-services through the REST interface of each micro-service.

![Physical Diagram](./physical.svg)

## Micro-Services
These are the micro-services for the subsystem. The combination of the micro-services help implement
the subsystem's logic.

### dev
Detail information for the [dev environment](environment--edgemere-diml-ddf-dr-dev)
can be found [here](environment--edgemere-diml-ddf-dr-dev)

Services in the dev environment

* frontend : diml_ddf_dr_web
* gw : diml_ddf_dr_gw

### test
Detail information for the [test environment](environment--edgemere-diml-ddf-dr-test)
can be found [here](environment--edgemere-diml-ddf-dr-test)

Services in the test environment

* frontend : diml_ddf_dr_web
* gw : diml_ddf_dr_gw

### prod
Detail information for the [prod environment](environment--edgemere-diml-ddf-dr-prod)
can be found [here](environment--edgemere-diml-ddf-dr-prod)

Services in the prod environment

* frontend : diml_ddf_dr_web
* gw : diml_ddf_dr_gw


## Interface Details


