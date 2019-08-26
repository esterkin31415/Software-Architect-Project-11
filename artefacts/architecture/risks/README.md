# Risk Registrar

| Risk | Likelihood | Impact | Risk to Patients | Mitigation Strategy |
| ---- | ---------- | ------ | ---------------- | ------------------- |
| Real time emergency responder system does not scale with incidents | Unknown | High | High | Early performance testing of a representative proof of concept |
| Real time emergency responder does handle latency regarding bed availability from collaborating hospital systems |  Unknown | High | High | Early performance testing of a representative proof of concept |
| Real time emergency responder does not cope when there are no hospitals available for with a required specialisation | Unknown | High | High | Agree to fall back the closest hospital with beds |
| Real time emergency responder does not respond within 200 nanoseconds when asked to provide a bed| Unknown | High | High | Proof of concept an emergency end point to provide any hospital with a bed |
| Emergency responder system cannot be interfaced by other systems | Medium | Medium | Low | Utilise OpenAPI |
 