
---

## 2. Available Search Variables

### **Filename:** `AvailableVariables.md`

```markdown
# Available Search Variables

To help you effectively use the `GetClinicalTrialValue` function, here's a detailed list of all possible `searchVariable` inputs you can use, categorized by their respective modules and data areas.

### Identification Module

| **Search Variable**                | **Description**                                           |
|------------------------------------|-----------------------------------------------------------|
| `brieftitle`                       | Retrieves the brief title of the clinical study.          |
| `officialtitle`                    | Retrieves the official title of the clinical study.       |
| `acronym`                          | Retrieves the acronym associated with the study.          |
| `nctid`                            | Retrieves the unique NCT Identifier of the study.         |
| `leadsponsorname`                  | Retrieves the name of the lead sponsor organization.      |
| `leadsponsorclass`                 | Retrieves the classification of the lead sponsor.         |
| `responsiblepartytype`             | Retrieves the type of the responsible party.              |
| `responsiblepartyinvestigatorfullname` | Retrieves the full name of the responsible party investigator. |
| `responsiblepartyinvestigatortitle`    | Retrieves the title of the responsible party investigator. |
| `responsiblepartyinvestigatoraffiliation` | Retrieves the affiliation of the responsible party investigator. |
| `responsiblepartyoldnametitle`        | Retrieves the old name/title of the responsible party.  |
| `responsiblepartyoldorganization`     | Retrieves the old organization of the responsible party.|

### Status Module

| **Search Variable**     | **Description**                                                   |
|-------------------------|-------------------------------------------------------------------|
| `overallstatus`         | Retrieves the overall status of the study (e.g., Completed, Recruiting). |
| `startdate`             | Retrieves the start date of the study.                            |
| `startdatetype`         | Retrieves the type of start date (e.g., Actual, Estimated).       |
| `completiondate`        | Retrieves the completion date of the study.                       |
| `completiondatetype`    | Retrieves the type of completion date (e.g., Actual, Estimated).  |
| `primarycompletiondate` | Retrieves the primary completion date and its type, concatenated.  |
| `studyfirstsubmitdate`  | Retrieves the date when the study was first submitted.            |
| `studyfirstsubmitqcdate`| Retrieves the date of the first quality control submission.       |
| `studyfirstpostdate`    | Retrieves the first post date and its type, concatenated.         |
| `lastupdatesubmitdate`  | Retrieves the date when the last update was submitted.            |
| `lastupdatepostdate`    | Retrieves the last update post date and its type, concatenated.   |

### Description Module

| **Search Variable**     | **Description**                                           |
|-------------------------|-----------------------------------------------------------|
| `briefsummary`          | Retrieves a brief summary of the study.                   |
| `detaileddescription`   | Retrieves a detailed description of the study.            |

### Conditions Module

| **Search Variable** | **Description**                                           |
|---------------------|-----------------------------------------------------------|
| `conditions`        | Retrieves a list of conditions being studied.            |

### Design Module

| **Search Variable**           | **Description**                                               |
|-------------------------------|---------------------------------------------------------------|
| `studytype`                   | Retrieves the type of study (e.g., Interventional, Observational). |
| `numphases`                   | Retrieves the number of phases in the study.                 |
| `designallocation`            | Retrieves the allocation method (e.g., Randomized).          |
| `designinterventionmodel`     | Retrieves the intervention model (e.g., Parallel).           |
| `designinterventionmodeldescription` | Retrieves a description of the intervention model.    |
| `designprimarypurpose`        | Retrieves the primary purpose of the study (e.g., Prevention).|
| `designobservationalmodel`    | Retrieves the observational model (if applicable).           |
| `designtimeperspective`       | Retrieves the time perspective of the study.                 |
| `designmasking`               | Retrieves details about masking in the study (e.g., Single, Double). |
| `designmaskingdescription`    | Retrieves a description of the masking method.               |
| `designwhomasked`             | Retrieves entities that are masked (e.g., Participant, Investigator). |

### Eligibility Module

| **Search Variable**           | **Description**                                           |
|-------------------------------|-----------------------------------------------------------|
| `eligibilitycriteria`         | Retrieves the criteria for eligibility in the study.      |
| `healthyvolunteers`           | Indicates if healthy volunteers are allowed in the study. |
| `sex`                         | Retrieves sex eligibility criteria (e.g., All, Male, Female). |
| `genderbased`                 | Indicates whether the study is gender-based.              |
| `genderdescription`           | Retrieves a description of the gender criteria.           |
| `minimumage`                  | Retrieves the minimum age requirement for participants.    |
| `maximumage`                  | Retrieves the maximum age limit for participants.          |
| `stdages`                     | Retrieves standardized age categories.                    |
| `studypopulation`             | Retrieves a description of the study population.           |
| `samplingmethod`              | Retrieves the method used for sampling participants.      |

### ContactsLocations Module

| **Search Variable**       | **Description**                                           |
|---------------------------|-----------------------------------------------------------|
| `overallofficialname`     | Retrieves the name of the overall official contact.       |
| `overallofficialaffiliation` | Retrieves the affiliation of the overall official contact. |
| `overallofficialrole`     | Retrieves the role of the overall official contact.       |
| `locationfacility`        | Retrieves the facility where the study is located.        |
| `locationcity`            | Retrieves the city where the study is conducted.          |
| `locationstate`           | Retrieves the state where the study is conducted.         |
| `locationzip`             | Retrieves the ZIP code of the study location.             |
| `locationcountry`         | Retrieves the country where the study is conducted.       |

### Outcomes Module

| **Search Variable** | **Description**                                           |
|---------------------|-----------------------------------------------------------|
| `primaryoutcome`    | Retrieves primary outcomes measured in the study.         |
| `secondaryoutcome`  | Retrieves secondary outcomes measured in the study.       |
| `otheroutcome`      | Retrieves other outcomes measured in the study.           |

### ArmsInterventions Module

| **Search Variable** | **Description**                                           |
|---------------------|-----------------------------------------------------------|
| `armgrouplabel`     | Retrieves labels of the arm groups in the study.          |
| `interventionname`  | Retrieves names of the interventions used in the study.   |

---

## Additional Notes

- **Case Sensitivity:** The `searchVariable` inputs are case-insensitive. You can enter them in uppercase, lowercase, or any combination thereof.
  
- **Handling Multiple Entries:** For fields that return multiple entries (e.g., `conditions`, `primaryoutcome`, `armgrouplabel`), the results will be concatenated and separated by commas or semicolons as appropriate.
  
- **Error Messages:**
  - If a `searchVariable` does not match any of the available options, the function will return "Invalid Search Variable".
  - If the requested field is not found or is empty, the function will return "Field not found or empty."

---

## Contact

For any questions, feedback, or support, please reach out to:

- **Name:** [Your Name]
- **Email:** [your.email@example.com]
- **GitHub:** [Your GitHub Profile](https://github.com/yourusername)
- **Website:** [Your Website](https://yourwebsite.com)

---

## License

This project is licensed under the [MIT License](LICENSE).

---
