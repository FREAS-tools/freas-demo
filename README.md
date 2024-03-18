# Demonstration Project for FREAS

[Modeller](https://github.com/FREAS-tools/freas-bpmn4frss-react) - Front-end web editor for BPMN4FRSS models

[Rule-Based Analyser](https://github.com/FREAS-tools/freas-analyzer-validity) - BPMN4FRSS model analyzer based on Z3

This repository serves as a demonstration of FREAS on the Automated Valet Parking (AVP) system (see https://doi.org/10.1145/3465481.3470052 for details). It consists of two models describing two iterations of a forensic-ready AVP system.

The first iteration (`avp_issuing_permit_1iteration.bpmn`) contains an error in the model. Furthermore, multiple design weaknesses are also present. The analyser highlights them so that a designer can resolve the errors and consider the possible weak points. To see the output, please run Validity and Hint analysis in FREAS.

In the second iteration (`avp_issuing_permit_2iteration.bpmn`), the error is resolved, together with several weak points hinted by the analyser. To see the difference, please run the Validity and Hint analysis in FREAS again. Now, the designer checks whether there is supporting evidence stored in the AVP system in these cases:
* A malicious insider injects a *Parking permit* into the *PLT parking permit storage* due to their permissions. Leading to loss of *Parking permit* integrity.
* An attacker fabricates a *Parking reservation* and sends it to the *PLT* interface due to missing access control. Leading to loss of *Parking permit* integrity.

Thus, the designer uses Evidence Quality analysis to check the supporting evidence if the *Parking reservation received* event (ID: `IntermediateThrowEvent_0qu79dp`) or the *PLT parking permit storage* data store reference (ID: `DataStoreReference_1o9b6q1`) are compromised. To see the output, please run Evidence Quality analysis in FREAS for both cases.

## Running FREAS
Use docker compose to run FREAS
```
docker compose up
```