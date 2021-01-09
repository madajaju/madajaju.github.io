---
layout: default
title: Package Provision Engine
permalink: package--edgemere-sml-pe
---
# Provision Engine

Provision Engine is a subsystem that provisions services onto the resources. It should provision everything necessary for the service to be deployed. Including but not limited to OS, libraries, security patches, monitoring etc...



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
The Data Model for the  Provision Engine shows how the different objects and classes of object interact
and their structure.

![Sub Package Diagram](./subpackage.svg)

### Sub Packages



![Logical Diagram](./logical.svg)

### Classes



## Activities and Flows
The Provision Engine subsystem provides the following activities and flows.

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

The Provision Engine subsystem is is physically laid out on a hybrid cloud infrastructure. Each microservice is shown
how they connect to each other. All of the micro-services communicate to each other and the main app through a
REST interface. A CLI, REST or Web interface for the app is how other subsystems or actors interact. Requests are
forwarded to micro-services through the REST interface of each micro-service.

![Physical Diagram](./physical.svg)

## Micro-Services
These are the micro-services for the subsystem. The combination of the micro-services help implement
the subsystem's logic.

### dev
Detail information for the [dev environment](environment--edgemere-sml-pe-dev)
can be found [here](environment--edgemere-sml-pe-dev)

Services in the dev environment

* frontend : sml_pe_web
* gw : sml_pe_gw

### test
Detail information for the [test environment](environment--edgemere-sml-pe-test)
can be found [here](environment--edgemere-sml-pe-test)

Services in the test environment

* frontend : sml_pe_web
* gw : sml_pe_gw

### prod
Detail information for the [prod environment](environment--edgemere-sml-pe-prod)
can be found [here](environment--edgemere-sml-pe-prod)

Services in the prod environment

* frontend : sml_pe_web
* gw : sml_pe_gw


## Interface Details


