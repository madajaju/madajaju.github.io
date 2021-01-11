---
layout: default
title: Data Scientist
permalink: actor-datascientist
parent: All Actors
---

# Data Scientist

Responsible for the architecture and development of data analytic models and solutions. They work closely with the Data engineer to deliver solutions to the Data Analyst.

There are several users of the system. We first took a use case analysis approach to the architecture. First,
identifying the actors/users of the system and building out how the actor uses the system? What their key objectives and
goals are? and How they use the system? This list is not an exhaustive list of all actors of the system but are the
primary actors.

These actors are found in most organizations and there are several different organizational structures that can be
employed. The key is to identify the people or organization that fits the different actors in the systems. The following
is an example of a centralized organizational structure of the actors of the system.

![Organization Layout](./orgchart.png)


## Use Cases

* [Manage AI Models](usecase-ManageAIModels)
* [Manage Data](usecase-ManageData)
* [Manage Data Adaptors](usecase-ManageDataAdaptors)
* [Manage Data Blue Prints](usecase-ManageDataBluePrints)
* [Manage Meta Data](usecase-ManageMetaData)
* [Manage Data Instances](usecase-ManageDataInstances)

  
![Use Case Diagram](./usecase.svg)

## User Interface
TBD

## Command Line Interface
* [ edgemere aml aimodel/list](action--edgemere-aml-aimodel-list) - Data Scientist manages AI models and ties them to and application and data set. DevOps will make sure when applications and AI models are updated that they are updatedtogether.
* [ edgemere diml cds data/list](action--edgemere-diml-cds-data-list) - Manage Data is the description
* [ edgemere diml ddf datadaptor/list](action--edgemere-diml-ddf-datadaptor-list) - Manage Data Adaptors is the description
* [ edgemere diml ddf datablueprint/list](action--edgemere-diml-ddf-datablueprint-list) - Manage Data Blue Prints is the description
* [ edgemere diml ddf metadata/list](action--edgemere-diml-ddf-metadata-list) - Manage Meta Data is the description
* [ edgemere diml dml do datainstance/list](action--edgemere-diml-dml-do-datainstance-list) - Manage Data Instances is the description

