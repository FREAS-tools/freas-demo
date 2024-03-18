# Example Models

The models are based on Automated Valet Parking Scenario: Issuing a Permit (see: https://doi.org/10.1145/3465481.3470052). They demonstrate the analyser in various cases.

* `avp_issuing_permit_full` - Full BPMN model.
* `avp_issuing_permit_simple` - Simplified BPMN model of Automated Valet Parking Scenario: Issuing a Permit. Enhanced with BPMN4FRSS constructs. 
* `avp_issuing_permit_log_storage` - Evidence Quality Analysis demonstration. Shows supporting potential evidence if *PLT parking permit storage* is compromised.
* `avp_issuing_permit_no_reservation_storage` - Evidence Quality Analysis demonstration. Shows no supporting potential evidence if *Parking reservation received* is compromised.
* `avp_issuing_permit_reservation_storage` - Evidence Quality Analysis demonstration. Shows supporting potential evidence if *Parking reservation received* is compromised.
* `avp_issuing_permit_missing_pes` - Hint Analysis demonstration. Shows that the *Parking permit* is missing a potential evidence source.