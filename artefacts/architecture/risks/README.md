# Risk Register

| Risk | Likelihood | Impact | Risk to Patients | Mitigation Strategy |
| ---- | ---------- | ------ | ---------------- | ------------------- |
| Real time emergency responder system does not scale with incidents | Unknown | High | High | Early performance testing of a representative proof of concept |
| Real time emergency responder does handle latency regarding bed availability from collaborating hospital systems |  Unknown | High | High | Early performance testing of a representative proof of concept |
| Real time emergency responder does not cope when there are no hospitals available for with a required specialisation | Unknown | High | High | Agree to fall back the closest hospital with beds |
| Real time emergency responder does not respond within 200 milliseconds when asked to provide a bed| Unknown | High | High | Proof of concept to prove an 'emergency' endpoint can provide **any** the responder with the name of any hospital with a bed in under 200 nanoseconds, during high load |
| Emergency responder system cannot be interfaced by other systems | Medium | Medium | Low | Utilise OpenAPI to define service contracts. Do so with the first proof of concept in order to demonstrate this and later customise it as a solution building block |
 