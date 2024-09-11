# Segmentation in Suffolk and North East Essex

This page lays out the technical logic and definitions that underpin the Suffolk and North East Essex Integrated Care System population segmentation model.

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
|Stay well|4|[One to three LTCs](#one-to-three-ltcs), [Cancer](#cancer), [Moderate frailty](#moderate-frailty)|
|Feel well|5|[Serious mental illness](), [Depression](#depression), [Anxiety](#anxiety), [Care contact for mental health](#care-contact-for-mental-health), [Hospitalised for mental health](#hospitalised-for-mental-health), [Hospitalised for alcohol](#hospitalised-for-alcohol), [Hospitalised for drugs](#hospitalised-for-drugs), [Hospitalised for self-harm](#hospitalised-for-self-harm), [Hospitalised for homelessness](#hospitalised-for-homelessness)|
|Be well|6| |
|Live well|7| Does not meet the criteria for any other segment.|

## Segment element definitions

Each segment element comprises of a codelist one or more clinical codes. These definitions are provided below. Where possible, definitions are taken from [primary care domain reference set clusters](https://digital.nhs.uk/data-and-information/data-collections-and-data-sets/data-collections/quality-and-outcomes-framework-qof/quality-and-outcome-framework-qof-business-rules/primary-care-domain-reference-set-portal). Where this is not possible, manual codelists are provided.

### Anxiety

- **Codelist:** opensafely/anxiety-disorders
- **Coding scheme:** SNOMED CT
- **Source:** [Open codelists](https://www.opencodelists.org/codelist/opensafely/anxiety-disorders/6aef605a/)
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Cancer

- **Codelist:** CAN_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Care contact for mental health

- **Codelist:** ind_cc_mh
- **Coding scheme:** NA
- **Source:** PCD Refset Cluster
- **Datasets:** MHSDS
- **Rules:** Any care contact within MHSDS in last year

### Dementia

- **Codelist:** DEM_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Depression

- **Codelist:** DEPR_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### End of life

- **Codelist:** ind_eol
- **Coding scheme:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### End stage COPD

- **Codelist:** ind_end_stage_COPD
- **Coding scheme:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### End stage heart disease

- **Codelist:** ind_end_stage_heart
- **Coding scheme:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### End stage liver disease

- **Codelist:** ind_end_stage_liver
- **Coding scheme:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### End stage renal disease

- **Codelist:** ind_end_stage_renal
- **Coding scheme:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Four or more LTCs

- **Codelist:** [Long-term conditions](ltc.md)
- **Coding scheme:** SNOMED CT
- **Source:**  [Long-term conditions](ltc.md)
- **Datasets:** Primary care
- **Rules:** Any code in codelist for at least four LTCs

### Has a carer

- **Codelist:** ind_has_carer
- **Coding scheme:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Hospitalised for alcohol

- **Codelist:** ind_hosp_alcohol
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year

### Hospitalised for asthma (under 24)

- **Codelist:** ind_hosp_asthma_under24
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year, and patient aged under 24

### Hospitalised for a fall

- **Codelist:** ind_hosp_fall
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year

### Hospitalised for drugs

- **Codelist:** ind_hosp_drug
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year

### Hospitalised for frailty

- **Codelist:** ind_hosp_frailty
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year

### Hospitalised for hip fracture

- **Codelist:** ind_hosp_hip
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year

### Hospitalised for homelessness

- **Codelist:** ind_hosp_homeless
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year

### Hospitalised for mental health

- **Codelist:** ind_hosp_mh
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year

### Hospitalised for mental health (under 24)

- **Codelist:** ind_hosp_mh_under24
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year, and patient aged under 24

### Hospitalised for self-harm

- **Codelist:** ind_hosp_selfharm
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year

### Hospitalised for self-harm (under 24)

- **Codelist:** ind_hosp_selfharm_under24
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year, and patient aged under 24

### Hospitalised for stroke

- **Codelist:** ind_hosp_stroke
- **Coding scheme:** SNOMED CT, ICD10
- **Source:** Forthcoming
- **Datasets:** SUS
- **Rules:** Any A&E attendance or admission with code in codelist within last year

### Housebound

- **Codelist:** ind_housebound
- **Coding scheme:** SNOMED CT
- **Source:** Forthcoming
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Moderate frailty

- **Codelist:** MODFRAIL_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### One to three LTCs

- **Codelist:** [Long-term conditions](ltc.md)
- **Coding scheme:** SNOMED CT
- **Source:**  [Long-term conditions](ltc.md)
- **Datasets:** Primary care
- **Rules:** Any code in codelist for one, two or three LTCs

### Palliative care

- **Codelist:** PALCARE_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Serious mental illness

- **Codelist:** MH_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Severe frailty

- **Codelist:** SEVFRAIL_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset Cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist