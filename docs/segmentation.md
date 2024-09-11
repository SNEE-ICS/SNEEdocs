# Segmentation in Suffolk and North East Essex

## Model structure and logic

## Segment definitions

|Segment Name|Segment priority|Segment elements|
|---|---|---|
|Die well|1|[Palliative care](#palliative-care), [End of life](#end-of-life), [End stage liver disease](#end-stage-liver-disease), [End stage heart disease](#end-stage-heart-disease), [End stage renal disease](#end-stage-renal-disease), [End stage COPD](#end-stage-copd)|
|Start well|2|[Hospitalised for asthma (under 24)](#hospitalised-for-asthma-under-24), [Hospitalised for self-harm (under 24)](#hospitalised-for-self-harm-under-24), [Hospitalised for mental health (under 24)](#hospitalised-for-mental-health-under-24)|



## Segment element definitions

Each segment element comprises of a codelist one or more clinical codes. These definitions are provided below. Where possible, definitions are taken from [primary care domain reference set clusters](https://digital.nhs.uk/data-and-information/data-collections-and-data-sets/data-collections/quality-and-outcomes-framework-qof/quality-and-outcome-framework-qof-business-rules/primary-care-domain-reference-set-portal). Where this is not possible, manual codelists are provided.

### End of life

- **Codelist:** ind_eol
- **Type:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### End stage COPD

- **Codelist:** ind_end_stage_COPD
- **Type:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### End stage heart disease

- **Codelist:** ind_end_stage_heart
- **Type:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### End stage liver disease

- **Codelist:** ind_end_stage_liver
- **Type:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### End stage renal disease

- **Codelist:** ind_end_stage_renal
- **Type:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Hospitalised for asthma (under 24)

- **Codelist:** ind_hosp_asthma_under24
- **Type:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any code in codelist and patient aged under 24

### Hospitalised for self-harm (under 24)

- **Codelist:** ind_hosp_selfharm_under24
- **Type:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any code in codelist and patient aged under 24

### Hospitalised for mental health (under 24)

- **Codelist:** ind_hosp_mh_under24
- **Type:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any code in codelist and patient aged under 24

### Palliative care

- **Codelist:** PALCARE_COD
- **Type:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist