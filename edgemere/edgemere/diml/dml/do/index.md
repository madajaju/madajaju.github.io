---
layout: default
title: Package Data Orchestrator
permalink: package--edgemere-diml-dml-do
---
# Data Orchestrator

Data Orchestrator is a package that contains...



## Use Cases

* [Manage Data Instances](usecase-ManageDataInstances)


![UseCase Diagram](./usecases.svg)

## Users
* [DataScientist](actor-datascientist)
* [ApplicationDeveloper](actor-applicationdeveloper)


![User Interaction](./userinteraction.svg)

## Interface
The subsystem has a REST, CLI, WebSocket, and Web interface. Use Cases and Scenarios can use any or all
of the interfaces to perform the work that needs to be completed. The following  diagram shows how
users interact with the system.

![Scenario Mappings Diagram](./scenariomapping.svg)

* [ edgemere diml dml do evaluate](#action--edgemere-diml-dml-do-evaluate)
* [ edgemere diml dml do reserve](#action--edgemere-diml-dml-do-reserve)
* [ edgemere diml dml do datainstance create](#action--edgemere-diml-dml-do-datainstance-create)
* [ edgemere diml dml do datainstance destroy](#action--edgemere-diml-dml-do-datainstance-destroy)
* [ edgemere diml dml do datainstance find](#action--edgemere-diml-dml-do-datainstance-find)
* [ edgemere diml dml do datainstance list](#action--edgemere-diml-dml-do-datainstance-list)


## Logical Artifacts
The Data Model for the  Data Orchestrator shows how the different objects and classes of object interact
and their structure.

![Sub Package Diagram](./subpackage.svg)

### Sub Packages



![Logical Diagram](./logical.svg)

### Classes

* [DataInstance](class-DataInstance)
* [DataRequest](class-DataRequest)
* [DataReservation](class-DataReservation)


## Activities and Flows
The Data Orchestrator subsystem provides the following activities and flows.

### Messages Handled
| Message | Action | Description |
|---|---|---|
| datareference.provisioning | /diml/dml/do/datainstance/create |  |
| datarequest.needed | /diml/dml/do/reserve |  |
| datarequest.selected | /diml/dml/do/evaluate |  |

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

The Data Orchestrator subsystem is is physically laid out on a hybrid cloud infrastructure. Each microservice is shown
how they connect to each other. All of the micro-services communicate to each other and the main app through a
REST interface. A CLI, REST or Web interface for the app is how other subsystems or actors interact. Requests are
forwarded to micro-services through the REST interface of each micro-service.

![Physical Diagram](./physical.svg)

## Micro-Services
These are the micro-services for the subsystem. The combination of the micro-services help implement
the subsystem's logic.

### dev
Detail information for the [dev environment](environment--edgemere-diml-dml-do-dev)
can be found [here](environment--edgemere-diml-dml-do-dev)

Services in the dev environment

* frontend : diml_dml_do_web
* gw : diml_dml_do_gw

### test
Detail information for the [test environment](environment--edgemere-diml-dml-do-test)
can be found [here](environment--edgemere-diml-dml-do-test)

Services in the test environment

* frontend : diml_dml_do_web
* gw : diml_dml_do_gw

### prod
Detail information for the [prod environment](environment--edgemere-diml-dml-do-prod)
can be found [here](environment--edgemere-diml-dml-do-prod)

Services in the prod environment

* frontend : diml_dml_do_web
* gw : diml_dml_do_gw


## Interface Details


### Action  edgemere diml dml do evaluate

* REST - /edgemere/diml/dml/do/evaluate
* bin -  edgemere diml dml do evaluate
* js - .edgemere.diml.dml.do.evaluate

Reserve a Data Instances from a Data Request

| Name | Type | Required | Description |
|---|---|---|---|
| request | ref |true | This is the data request to get the reservations |




### Action  edgemere diml dml do reserve

* REST - /edgemere/diml/dml/do/reserve
* bin -  edgemere diml dml do reserve
* js - .edgemere.diml.dml.do.reserve

Reserve a Data Instances from a Data Request

| Name | Type | Required | Description |
|---|---|---|---|
| request | ref |true | This is the data request to get the reservations |




### Action  edgemere diml dml do datainstance create

* REST - /edgemere/diml/dml/do/datainstance/create
* bin -  edgemere diml dml do datainstance create
* js - .edgemere.diml.dml.do.datainstance.create

Create a Data Instance from a Data Reference

| Name | Type | Required | Description |
|---|---|---|---|
| dataref | json |false | This is a Data Reference that should be turned into a Data Instance |




### Action  edgemere diml dml do datainstance destroy

* REST - /edgemere/diml/dml/do/datainstance/destroy
* bin -  edgemere diml dml do datainstance destroy
* js - .edgemere.diml.dml.do.datainstance.destroy

Description of the action

| Name | Type | Required | Description |
|---|---|---|---|
| attr1 | string |false | Description for the parameter |




### Action  edgemere diml dml do datainstance find

* REST - /edgemere/diml/dml/do/datainstance/find
* bin -  edgemere diml dml do datainstance find
* js - .edgemere.diml.dml.do.datainstance.find

Description of the action

| Name | Type | Required | Description |
|---|---|---|---|
| attr1 | string |false | Description for the parameter |




### Action  edgemere diml dml do datainstance list

* REST - /edgemere/diml/dml/do/datainstance/list
* bin -  edgemere diml dml do datainstance list
* js - .edgemere.diml.dml.do.datainstance.list

Description of the action

| Name | Type | Required | Description |
|---|---|---|---|
| attr1 | string |false | Description for the parameter |




