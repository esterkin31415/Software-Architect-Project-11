![MedHead Logo](../../../images/logo.png)
# Summary Statement of Architecture Work and Tailored Architecture
Project: Proof of Concept: Emergency Responder Hospital Bed Allocation 
Client: MedHead Consortium

# Table of Contents
* Project Request and Background
  * Overarching Context
  * Specific Request
  *  Strategic Alignment
  * Suggested Simplifications
* Objectives and Scope
* Architecture Approach
  * Architecture Process
  * Architecture Content
* Relevant Methodologies and Industry Standards
* Support of the Enterprise Continuum
* Work Deliverables
  * Duration and Effort
* Risks and Mitigation
* Acceptance Criteria and Procedures
* Metrics and KPIs
* Approvals

# Project Request and Background
## Overarching Context
See [Architecture Definition Document](../architecture-definition-document) where this content 
has been moved and is currently up to date.

## Specific Request
Based on identified project [risks](../risks/) the Architecture Advisory Board has requested
a learning spike which tests the hypothesis presented [here](../hypothesis-emergency-responder) 

##  Strategic Alignment
A learning centric proto-type will be built with a view to de-risking the emergency responder component
of the overall MedHead target state architecture:
![MedHead Target State Architecture](../../../images/target-state-architecture-vision.png)

## Suggested Simplifications
The proof of concept may simplify its responsibility to focus primarily on 
proving concerns laid out in the hypothesis. Examples of potential simplifications 
include:
* Only collaborating with stub interfaces or dummy implementations of collaborating systems.
* Making simplified assumptions about the contracts of these downstream systems.
* Documenting short-comings of a prototype and a plan to address these in any resulting systems. 
 
# Objectives and Scope
The business objectives of this architecture work are 
laid out in the [hypothesis to be satisifed by this brief](../hypothesis-emergency-responder) 

# Architecture Approach
## Architecture Process
The TOGAF Architecture Development Method (ADM) defines a best-practice methodology for architecture development. However, not all phases are necessarily equally relevant to every project. The table below describes the usage of the ADM for this particular project.


 |  Phase  |  In / Out  |  Notes  | 
 |  -----  |  --------  |  -----  | 
 |  Preliminary  |   |   | 
 |  A – Architecture Vision  | IN  | _consolidated into objectives of the PoC Hypothesis and Architecture Definition Document_ | 
 |  B – Business Architecture  |  IN |  **Parallelised with C and D:**, _Operates in the domain of Emergency Response and Bed Allocations_  | 
 |  C – Information Systems Architecture  |  IN  |  **Parallelised with B and D:**, _Operates in the domain of Emergency Response and Bed Allocations_, _Aim to adhere to appropriate [Architectural Principles](../architecture-principles/)_ |
 |  D – Technology Architecture  |   | **Parallelised with B and C:**, _Adheres to _  | 
 |  E – Opportunities and Solutions  | IN  | Focus on Solutions Architecture to satisfy testing the Hypothesis | 
 |  F – Migration Planning  | IN  | _Focus on defining building blocks for PoCs, path to production and building blocks for a CI/CD deployment pipeline._ | 
 |  G – Implementation Governance  |   | PoC may in this instance use Self-assessment based on Architectural Principles and focus on demonstrating conformance with PoC specific principles.| 
 |  H – Architecture Change Management  | IN  | Architecture updates are permitted and should be documented through an approval history of pull-requests to architectural components and other artefacts. | 

This first cycle will set a base-line for the approach used with Proof of Concepts. Learnings 
may be shared through an accompanying document containing notes on those learnings.

## Architecture Content

The TOGAF Architecture Content Framework (ACF) provides a best-practice categorization of architecture content. However, not all items are necessarily equally relevant to every project. The table below describes the content areas relevant to this particular project.


 |  Content Area  |  In / Out  |  Notes  | 
 |  -----  |  --------  |  -----  |
 |  Architecture Principles, Vision, and Requirements  |  IN |  Defined across [Architecture Principles](../architecture-principles), [Architecture Definition Document](../architecture-definition-document) and the [PoC Hypothesis](../hypothesis-emergency-responder)  | 
 |  Business Architecture  | IN  |  See high level Domain Model in the [Architecture Definition Document](../architecture-definition-document)  | 
 |  Information Systems Architecture – Data  | IN  | Update this SoW if necessary. See also [Architecture Definition Document](../architecture-definition-document) The Architecture Committee recommend a Data-Driven approach.  |  
 |  Information Systems Architecture – Applications  |   |  Update this SoW if necessary. See also [Architecture Definition Document](../architecture-definition-document)  |  
 |  Technology Architecture  | IN  |  Any updates to this document or the [Architecture Definition Document](../architecture-definition-document. Add a methodology and specification in the [PoC Hypothesis](../hypothesis-emergency-responder) document. | 
 |  Architecture Realisation  | IN  | Complete software project with a working and specified API, proven using sound engineering and testing principles. In code/project documentation to also be supplied in the repository. Markdown to be provided with a road-map to productionise or pivot, based on the learnings. | 

Key stake holder concerns should be addressed and given priority, particularly in relation to response times, scalability, tolerance of collaborator (hospital system) outages and resilience under load.  

# Relevant Methodologies and Industry Standards
See [Architecture Principles](../architecture-principles) and its specific principles for Proofs of Concept.

# Support of the Enterprise and Solution Continuum
Where possible the PoC should aim to either provide or facilitate the provision of Solution and Architecture Building 
Blocks which may benefit future Proof of Concepts and other engineering efforts.

Specifically we would like the PoC to produce:
* A testing strategy for proof of concepts.
* A test plan documented in the project which can inform other Proofs of Concepts.
* Demonstration of a CI/CD pattern which can be used for other projects.

# Work Deliverables

* A working implementation, tests with supporting documentation.
* Test Execution reports produced during continuous integration to demonstrate delivered behaviours.
* A presentation of the PoC, proof of supported behaviour, learnings and future recommendations.

## Duration and Effort

Discuss with leadership team.

# Risks and Mitigation
See the [Risk Register](../risks)

# Acceptance Criteria and Procedures
# Metrics and KPIs
Please define appropriately inline with the [PoC Hypothesis](../hypothesis-emergency-responder) and [Architecture Principles](../architecture-principles).

# Approvals

Kara Trace, *MedHead Board of Trustees*
