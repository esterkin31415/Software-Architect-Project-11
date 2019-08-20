![MedHead Logo](../../../images/logo.png)
# Architecture Definition Document

# Executive Summary 

This document details the base line architectures, business proposition, target architecture vision, migration requirements and provides a gap analysis between the two.

# Purpose

The Architecture Definition Document is the deliverable container for the core architectural artifacts created during this project. The Architecture Definition Document spans all architecture domains (business, data, application, and technology) and also examines all relevant states of the architecture (baseline, interim state(s), and target).

The Architecture Definition Document is a companion to the Architecture Requirements Specification (yet to be prepared for this project), with a complementary objective:
* The Architecture Definition Document provides a qualitative view of the solution and aims to communicate the intent of the architects.
* The Architecture Requirements Specification provides a quantitative view of the solution, stating measurable criteria that must be met during the implementation of the architecture.

_It is suggested that this document reference the various deliverables in the container. For instance, the Architecture Principles will be documented in an Architecture Principles document and that document referenced here. It may be that this container is implemented using a wiki or as an intranet rather than a text-based document. Even better would be to use a licensed TOGAF tool that captures this output._

_This template shows “typical” contents of an Architecture Definition Document and can be adapted to align with any TOGAF adaptation being implemented._

# Target Audiance
This deliverable is intended to be consumed by all pesonel involved in the project. It defines a vision and high-level architecture which address the business drivers of the project.
This document therefore should act as an input into further stages of elaboration, with new insights back-propagated as revisions to this document.

# Business Context and Drivers

A consortium of four leading companies have come together to consolidate their efforts, data, applications and roadmaps in order to develop a next generation patient centric platform capable of improving base-line patient care, while also being responsive and capable of, real-time, information based decision making in emergency situations.

The following organisations bring data specialisation and patient centric expertease in each of the following domains.

| *Organisation* | *Specialist Domain* | *Business Motivations* | *Notes* |
| -------------- | ------------------- | ---------------------- | ------- |
| Ursa Major Health | GP Appointment Scheduling | Workflow enhancement around manual integration with other systems | Appointment consolidation and reducing integration issues with hospital appointment systems |
| Jupiter Scheduling | Hospital appointment scheduling | Workflow enhancement around manual integration with other systems | Synergies with other appointment systems and removal of manual integrations with GP scheduling systems |
| Emergency Expert Systems | Real time hospital recommendations based on bed availability | Data integration and quality required to improve decisions | Reduce rate of poor recommendations by weighing decisions based on the patients broader medical history. | 
| Schedule Shed | Medical staff rosters and scheduling | Workflow enhancement | Currently depends on unreliable manual updates of appointment systems when staff are not available |   

All parties in the consortium intend to reduce duplication of matching capabilities, whilst developing new capabilities which present opportunies to deliver value to patients through improved integration and data sharing between systems.   

The primary goal of the consolidated project is to evolve a service based platform which benefits from event streams between systems, enabling decoupled and fault-tolerant single responsibility services adhering to the [principles](../architecture-principles/) of a decomposed microsevice architecture.

# Scope and Project Aims

This project aims to deliver a target business state which results in a joint architectural governance function 
across the consortium, through a jointly owned Platform and Systems Management group which is intended to provide 
benefits from economies of scale and adherence to a strategic roadmap to 
delivering a platform which compromises business agility and time to market, with levels of data security and fault 
tolerance required of institutions in the health care sector.

The project will follow the ADM specified in the [Summary Statement of Work](../summary-statement-of-architecture-work)




