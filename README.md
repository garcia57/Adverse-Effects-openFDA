# Adverse-Effects-openFDA

## Dataset Description
This dataset provides detailed records of reported adverse drug events, including information on the patient demographics, event seriousness, drug characterization, and routes of administration.

## Column Descriptions

### serious
- <strong>Type</strong>: Integer (1 or 2)
  - 1: Serious event.
  - 2: Non-serious event.

- <strong>Description</strong>: Indicates the overall seriousness of the adverse event. For example, did the drug cause a life-threatening event, hospitiation, and/or result in a disability.


### seriousnessdeath

- <strong>Type</strong>: Binary (1 or 0)
  - 1: Resulted in death.
  - 0: Did not result in death.
- <strong>Description</strong>: Indicates if the adverse event resulted in the patient’s death.


### patient_sex

- <strong>Type</strong>: Integer (1 or 2)
  - 1: Male.
  - 2: Female.
- <strong>Description</strong>: Represents the sex of the patient.


### patient_age

- <strong>Type</strong>: Numeric

- <strong>Description</strong>: Age of the patient at the time of the adverse event. The age unit is provided in the next column.

### patient_age_unit

- <strong>Type</strong>: String or Numeric
  - Days, Weeks, Months, Years, Hours
  - NULL: When the age unit is missing.
- <strong>Description</strong>: The unit of measurement for patient_age.

### drug_characterization

- <strong>Type</strong>: Integer (1, 2, or 3)
  - 1: Causal (suspected cause of the event).
  - 2: Concurrent (taken concurrently but not suspected of causing the event).
  - 3: Synergistic (may have interacted with the causal drug).

- <strong>Description</strong>: Categorizes the drug’s role in the adverse event.


### drugadministrationroute

- <strong>Type</strong>: String or Numeric
  - Oral, Intravenous, Subcutaneous, Transdermal, etc.
  - NULL: When the route is missing.
- <strong>Description</strong>: The route of administration for the drug. 

### reaction_meddra

- <strong>Type</strong>: String

- <strong>Description</strong>: A standardized term from the Medical Dictionary for Regulatory Activities (MedDRA) describing the type of adverse reaction experienced by the patient.

## Summary
My hope for this small dataset is to provide a fruitful foundation for people to practice analyzing drug-related adverse events, with columns detailing the severity and type of event, patient demographics, drug roles, and methods of administration. This structure allows for in-depth analysis of factors contributing to serious adverse events and patterns across different drugs and patient profiles.
