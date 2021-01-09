---
layout: default
title: Package Common Data Service
permalink: package--edgemere-diml-cds
---
# Common Data Service

Common Data Service is a package that contains...



## Use Cases

* [Manage Data](usecase-ManageData)


![UseCase Diagram](./usecases.svg)

## Users
* [DataScientist](actor-datascientist)
* [DataAnalyst](actor-analyst)
* [DataEngineer](actor-dataengineer)


![User Interaction](./userinteraction.svg)

## Interface
The subsystem has a REST, CLI, WebSocket, and Web interface. Use Cases and Scenarios can use any or all
of the interfaces to perform the work that needs to be completed. The following  diagram shows how
users interact with the system.

![Scenario Mappings Diagram](./scenariomapping.svg)

* [ edgemere diml cds data list](#action--edgemere-diml-cds-data-list)
* [ edgemere diml cds data source name](#action--edgemere-diml-cds-data-source-name)


## Logical Artifacts
The Data Model for the  Common Data Service shows how the different objects and classes of object interact
and their structure.

![Sub Package Diagram](./subpackage.svg)

### Sub Packages

* [Ingress Services](package--edgemere-diml-cds-ingress)
* [Insite Services](package--edgemere-diml-cds-insite)
* [Storage Services](package--edgemere-diml-cds-storage)
* [Transform Services](package--edgemere-diml-cds-transform)


![Logical Diagram](./logical.svg)

### Classes



## Activities and Flows
The Common Data Service subsystem provides the following activities and flows.

### Messages Handled

| Message | Action | Description |
|---|---|---|


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

The Common Data Service subsystem is is physically laid out on a hybrid cloud infrastructure. Each microservice is shown
how they connect to each other. All of the micro-services communicate to each other and the main app through a
REST interface. A CLI, REST or Web interface for the app is how other subsystems or actors interact. Requests are
forwarded to micro-services through the REST interface of each micro-service.

![Physical Diagram](./physical.svg)

## Micro-Services
These are the micro-services for the subsystem. The combination of the micro-services help implement
the subsystem's logic.

### dev
Detail information for the [dev environment](environment--edgemere-diml-cds-dev)
can be found [here](environment--edgemere-diml-cds-dev)

Services in the dev environment

* frontend : diml_cds_web
* gw : diml_cds_gw

### test
Detail information for the [test environment](environment--edgemere-diml-cds-test)
can be found [here](environment--edgemere-diml-cds-test)

Services in the test environment

* frontend : diml_cds_web
* gw : diml_cds_gw

### prod
Detail information for the [prod environment](environment--edgemere-diml-cds-prod)
can be found [here](environment--edgemere-diml-cds-prod)

Services in the prod environment

* frontend : diml_cds_web
* gw : diml_cds_gw


## Interface Details


### Action  edgemere diml cds data list

* REST - /edgemere/diml/cds/data/list
* bin -  edgemere diml cds data list
* js - .edgemere.diml.cds.data.list

Description of the action

| Name | Type | Required | Description |
|---|---|---|---|
| attr1 | string |false | Description for the parameter |




### Action  edgemere diml cds data source name

* REST - /edgemere/diml/cds/data/source/name
* bin -  edgemere diml cds data source name
* js - .edgemere.diml.cds.data.source.name

Description of the action

| Name | Type | Required | Description |
|---|---|---|---|
| attr1 | string |false | Description for the parameter |




