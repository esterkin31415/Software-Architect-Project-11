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
* Instructions to productionise the proven pattern
* Implementation completed within an allocated time frame

# Example Behaviour and a Description of the Capability

The Real-Time Emergency Responder Sub-system is intended to receive one or more
more medical specialisms (See [Specialism Reference Data](../models/reference-data/specialities)) 
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

# Methodlogy

* TO be completed..

# Results

* TO be completed..