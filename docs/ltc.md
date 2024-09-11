![logo](assets/SNEE_IF_logo.png)

# Long-term conditions and complexity

This page outlines the long-term conditions used for the purposes of population health management analysis in the Suffolk and North East Essex Integrated Care System. Specifically, the below outlines the definitions of conditions that are used in our [segmentation model](segmentation.md), and the definitions of high, medium and low complexity. The below does not reflect any clinical judgement on what does and does not constitute a long-term condition, nor does it reflect which conditions are prioritised for healthcare services. It is a non-exhaustive list.

## Long-term condition list

- [Anxiety](#anxiety)
- [Asthma](#asthma)
- [Atrial fibriliation](#atrial-fibriliation)
- [Chronic kidney disease](#chronic-kidney-disease)
- [COPD](#copd)
- [Depression](#depression)
- [Diabetes](#diabetes)
- [Epilepsy](#epilepsy)
- [Heart failure](#heart-failure)
- [Hypertension](#hypertension)
- [Learning disability](#learning-disability)
- [Osteoporosis](#osteoporosis)
- [Peripheral vascular disease](#peripheral-vascular-disease)
- [Stroke](#stroke)
- [Transient ischaemic attack (TIA)](#transient-ischaemic-attack-tia)

## Complexity definitions

|Level|Definition|
|-|-|
|High complexity|Four or more LTCs|
|Medium complexity|One to three LTCs|
|Low complexity|No LTCs|

## Long-term condition definitions

### Anxiety

- **Codelist:** opensafely/anxiety-disorders
- **Resolved codelist:** NA
- **Coding scheme:** SNOMED CT
- **Source:** [Open codelists](https://www.opencodelists.org/codelist/opensafely/anxiety-disorders/6aef605a/)
- **Datasets:** Primary care
- **Rules:** Any code in codelist

### Asthma

- **Codelist:** AST_COD
- **Resolved codelist:** ASTRES_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Atrial fibriliation

- **Codelist:** AFIB_COD
- **Resolved codelist:** AFIBRES_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Chronic kidney disease

- **Codelist:** CKD_COD
- **Resolved codelist:** CKDRES_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### COPD

- **Codelist:** COPD_COD
- **Resolved codelist:** COPDRES_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Depression

- **Codelist:** DEPR_COD
- **Resolved codelist:** DEPRRES_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Diabetes

- **Codelist:** DM_COD
- **Resolved codelist:** DMRES_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Epilepsy

- **Codelist:** EPIL_COD
- **Resolved codelist:** EPILRES_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Heart failure

- **Codelist:** HF_COD
- **Resolved codelist:** HFRES_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Hypertension

- **Codelist:** HYP_COD
- **Resolved codelist:** HYPRES_COD
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Learning disability

- **Codelist:** LD_COD
- **Resolved codelist:** NA
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Osteoporosis

- **Codelist:** OSTEO_COD
- **Resolved codelist:** NA
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Peripheral vascular disease

- **Codelist:** PAD_COD
- **Resolved codelist:** NA
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Stroke

- **Codelist:** STRK_COD
- **Resolved codelist:** NA
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist

### Transient Ischaemic Attack (TIA)

- **Codelist:** TIA_COD
- **Resolved codelist:** NA
- **Coding scheme:** SNOMED CT
- **Source:** PCD Refset cluster
- **Datasets:** Primary care
- **Rules:** Any code in codelist that postdates any code in the resolved codelist