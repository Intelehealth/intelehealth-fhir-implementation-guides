# Patient Mapping between OpenMRS and FHIR

This section describes the mapping between the OpenMRS Patient profile and the FHIR Patient resource.

## Mapping Table

| **Source Element**                | **Target Element**            | **Mapping Name**        |
|-----------------------------------|-------------------------------|-------------------------|
| `OpenMRS.Patient.identifier`      | `Patient.identifier`          | `identifierMapping`     |
| `OpenMRS.Patient.id`              | `Patient.id`                  | `idMapping`             |
| `OpenMRS.Patient.name`            | `Patient.name`                | `nameMapping`           |
| `OpenMRS.Person.personAttribute`  | `Patient.telecom`             | `telecomMapping`        |
| `OpenMRS.Patient.gender`          | `Patient.gender`              | `genderMapping`         |
| `OpenMRS.Patient.birthDate`       | `Patient.birthDate`           | `birthDateMapping`      |
| `OpenMRS.Patient.deceased[x]`     | `Patient.deceased[x]`         | `deceasedMapping`       |
| `OpenMRS.Patient.address`         | `Patient.address`             | `addressMapping`        |
| `OpenMRS.Patient.active`          | `Patient.active`              | `activeMapping`         |

This table maps OpenMRS Patient fields to the equivalent FHIR Patient fields, helping implementers align the two systems.

