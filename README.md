# Demostration Project for FREAS

[Modeller](https://github.com/FREAS-tools/freas-bpmn4frss-react) - Front-end web editor for BPMN4FRSS models

[Rule-Based Analyser](https://github.com/FREAS-tools/freas-analyzer-validity) - BPMN4FRSS model analyzer based on Z3

## Running FREAS
Use docker compose to run FREAS
```
docker compose up
```

## Example Models
The following is a list of models that showcases the FREAS capabilities.

### AVP System Demo
A demonstration of FREAS on Automated Valet Parking (AVP) system.

The first iteration contains various errors and warnings from Validity and Hint analysis.

The second iteration fixes the errors and chosen warnings. It further demonstrates the Evidence Quality analysis on `IntermediateThrowEvent_0qu79dp` and `DataStoreReference_1o9b6q1`.