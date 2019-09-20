# Hypothesis for Developing a Proof of Concept for the Real-Time Emergency Responder Subsystem

# Hypothesis Statement

**We believe** that implementing a Proof of Concept for the Real-Time Emergency
Responder Subsystem

**For** the MedHead Consortium Enterprise Architecture Team

**Will achieve**
* Confidence around the simplicity of such a system
* Confidence around the ability of other systems to integrate with the Emergency Responder system.
* Confidence around the resilience and responsiveness of such a system under load

**We will know we have succeeded when we see:**
* A clear OpenAPI specification with 4 or fewer endpoints (including health checks)
* Sub 200 millisecond response time maintained under load of up to 800 requests per second, per service instance.
* An implementation which explains which standards it respects and why.
* Instructions to productionize the proven pattern
* Implementation completed within an allocated time frame

# Example Behaviour and a Description of the Capability

The Real-Time Emergency Responder Sub-system is intended to receive one or more medical specialisms (See [Specialism Reference Data](../models/reference-data/specialities)) 
and a data store of recent hospital information in order to suggest a hospital, with an available bed, which is associated with
    one or more matching specialisations.
    
   For example:
   
   GIVEN that we have three hospitals with
   
   | Hospital | Beds Available  | Specialisations |
   | -------- | --------------  | -------------- |
   | Fred Brooks Hospital | 2 | Cardiology, Immunology |
   | Julia Crusher Hospital | 0 | Cardiology |
   | Beverly Bashir Hospital | 5 | Immunology, Diagnostic Neuropathology |
   
   AND a patient requiring Cardiology care
   
   WHEN asking for Cardiology care
   
   THEN a referral to the Fred Brooks Hospital should be provided
   
   AND an event published to reserve a bed.


# Agreed Constraints

The following constraints and pointers were raised when defining this hypothesis:

* The solutions should provide a RESTful API which should: 
 * keep medical responders informed, in real-time, about:where they need to go and what they need to do
 , Ensure that any patient data is properly protected. 
* You'll additionally have to ensure that your POC is fully tested:
  * In line with the project's Architectural Principles
  * Automation tests reflecting the Testing Pyramid (unit, integration, acceptance, and E2E tests)
  * The project should document its acceptance tests using BDD within the project.
  * Stress tests to provide confidence of business continuity in high volume situations.
* To ensure that the POC can be easily integrated into future development 
work, you will need to:
   * Centralize your code
   * Make it easily shareable
   * Provision both continuous integration (CI) and CD (continuous delivery) pipelines.
     * Test Reports produced during CI should clearly indicate which acceptance tests have passed and failed.
   * Document your testing strategy.
* It is desirable that subsequent teams can utilize it as a building block for 
continued iteration of this and other POCs.
* The delivery should also provide clear follow-through instruction to ensure that 
the POC’s shortcomings are transparent and stake-holders are clear about high-level 
steps involved in productionising a solution for the concept you have proven.

The resulting documentation and POC will be presented to members of the Board of Trustees for the purpose of 
 demonstrating and explaining the learnings from the proof of concept.
* To demonstrate the delivered behaviour, CI/CD runs should produce inspectable test reports which can be shown during the presentation.


# Methodlogy

* TO be completed..

# Findings

* TO be completed..
