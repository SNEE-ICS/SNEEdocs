# Segmentation in Suffolk and North East Essex

This page lays out the technical logic and definitions that underpin Suffolk and North East Essex Integrated Care System population segmentation model.

## Model structure and logic

- A **segment** refers to a group of the population. In our model, every patient goes into one and only one segment.
- A segment is defined by **segment elements**. Each segment element is a rule or set of related rules that can be evaluated as true or false. A patient meets the criteria for a segment if they meet the criteria for any segment element within that segment. 
- **Segment priority** is used to deal with overlap. If a patient meets the criteria to fit into more than one segment, they go into the highest priority segment.


## Segment definitions

|Segment Name|Segment priority|Segment elements|
|---|---|---|
|Die well|1|[Palliative care](#palliative-care), [End of life](#end-of-life), [End stage liver disease](#end-stage-liver-disease), [End stage heart disease](#end-stage-heart-disease), [End stage renal disease](#end-stage-renal-disease), [End stage COPD](#end-stage-copd)|
|Start well|2|[Hospitalised for asthma (under 24)](#hospitalised-for-asthma-under-24), [Hospitalised for self-harm (under 24)](#hospitalised-for-self-harm-under-24), [Hospitalised for mental health (under 24)](#hospitalised-for-mental-health-under-24)|
|Age well|3|[Hospitalised for hip fracture](#hospitalised-for-hip-fracture), [Hospitalised for stroke](#hospitalised-for-stroke), [Hospitalised for a fall](#hospitalised-for-a-fall), [Hospitalised for frailty](#hospitalised-for-frailty), [Dementia](#dementia), [Four or more LTCs](#four-or-more-ltcs), [Severe frailty](#severe-frailty), [Housebound](#housebound), [Has a carer](#has-a-carer)|
|Stay well|4| |
|Feel well|5| |
|Be well|6| |
|Live well|7| Does not meet the criteria for any other segment.|

## Segment element definitions

Each segment element comprises of a codelist one or more clinical codes. These definitions are provided below. Where possible, definitions are taken from [primary care domain reference set clusters](https://digital.nhs.uk/data-and-information/data-collections-and-data-sets/data-collections/quality-and-outcomes-framework-qof/quality-and-outcome-framework-qof-business-rules/primary-care-domain-reference-set-portal). Where this is not possible, manual codelists are provided.

### Dementia

- **Codelist:** DEM_COD
- **Type:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist

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

### Four or more LTCs

- **Codelist:** [Long-term conditions](ltc.md)
- **Type:** SNOMED CT
- **Source:**  [Long-term conditions](ltc.md)
- **Datasets:** Primary care
- **Rules:** Any code in codelist for at least four LTCs

### Has a carer

- **Codelist:** ind_has_carer
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

### Hospitalised for a fall

- **Codelist:** ind_hosp_fall
- **Type:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any code in codelist

### Hospitalised for frailty

- **Codelist:** ind_hosp_frailty
- **Type:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any code in codelist

### Hospitalised for hip fracture

- **Codelist:** ind_hosp_hip
- **Type:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any code in codelist

### Hospitalised for mental health (under 24)

- **Codelist:** ind_hosp_mh_under24
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

### Hospitalised for stroke

- **Codelist:** ind_hosp_stroke
- **Type:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any code in codelist

### Housebound

- **Codelist:** ind_housebound
- **Type:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Palliative care

- **Codelist:** PALCARE_COD
- **Type:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Severe frailty

- **Codelist:** SEVFRAIL_COD
- **Type:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist