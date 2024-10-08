![logo](assets/SNEE_IF_logo.png)

# Activity types and cost

This page contains our methodology for estimating costs of health activity. Note that these costs are used to compare healthcare activity across different sectors, and do not reflect actual expenditure. Click on the links in the table below to see methodology for individual cost estimates.

## Activity types and cost table

|Dataset|Activity type|Activity subtype|Cost per day|
|-------|------------|----------------|----|
|SUS|Acute AE|AE|Row level costings|
|SUS|Acute inpatient|Emergency|Row level costings|
|SUS|Acute inpatient|Elective|Row level costings|
|SUS|Acute inpatient|Non-elective non-emergency|Row level costings|
|SUS|Acute outpatient|First|Row level costings|
|SUS|Acute outpatient|Follow up|Row level costings|
|MHSDS|Mental health|Inpatient|[£564](#mental-health-inpatient)|
|MHSDS|Mental health|Care contact|[£275](#mental-health-care-contact)|
|IAPT|IAPT|Care contact|[£139](#iapt-care-contact)|
|Primary care|Primary care|Telephone/video appointment|[£45](#primary-care-telephonevideo-appointment)|
|Primary care|Primary care|Face to face appointment|[£51](#primary-care-face-to-face-appointment)|
|Primary care|Primary care|Written appointment|[£45](#primary-care-written-appointment)|
|CSDS|Community|Care contact|[£84](#community-care-contact)|
|CLD|Adult social care|Review|[£45](#adult-social-care-review)|
|CLD|Adult social care|Request|[£45](#adult-social-care-request)|
|CLD|Adult social care|Assessment|[£45](#adult-social-care-assessment)| 
|CLD|Adult social care|Carer support|[£20](#adult-social-care-carer-support)|
|CLD|Adult social care|Long-term support: community|[£62](#adult-social-care-long-term-support-community)|
|CLD|Adult social care|Long-term support: Residential home|[£149](#adult-social-care-long-term-support-residential-home)|
|CLD|Adult social care|Long-term support: Nusing home|[£173](#adult-social-care-long-term-support-nursing-home)|
|CLD|Adult social care|Short-term support|[£160](#adult-social-care-short-term-support)|

## Methodology

All costs are expressed in 2024 prices, and are [adjusted for inflation (CPI)](https://www.ons.gov.uk/economy/inflationandpriceindices/bulletins/consumerpriceinflation/may2024) as necessary.

### SUS

All acute activity and associated costs are populated from our patient-level [commissioning datasets](https://digital.nhs.uk/data-and-information/data-collections-and-data-sets/data-sets/commissioning-data-sets) which are submited to the secondary use services (SUS) repository. Activity-level costing data is provided as part of these datasets.

### MHSDS

Our mental health activity is estimates using the [mental health services dataset (MHSDS)](https://digital.nhs.uk/data-and-information/data-collections-and-data-sets/data-sets/mental-health-services-data-set). As yet, no activity-level costing data is available with this dataset, so we use our own costs based on activity types.

### Mental health inpatient

We have been unable to find good data on the cost per day of mental health inpatient stays. Our best source is a [freedom of information request](https://www.elft.nhs.uk/sites/default/files/2022-01/anon_response_-_foi_da3620.pdf) to East London NHS Foundation Trust, which we have adjusted for inflation. All costs are rounded to the nearest pound.


### Mental health care contact

[PSSRU Unit costs of social care](https://www.pssru.ac.uk/project-pages/unit-costs/) from 2022-23, adjusted for inflation

## IAPT (talking therapies)

Talking therapies activity is estimated using the [IAPT commissioning dataset](https://digital.nhs.uk/data-and-information/data-collections-and-data-sets/data-sets/improving-access-to-psychological-therapies-data-set).

### IAPT care contact

[PSSRU Unit costs of social care](https://www.pssru.ac.uk/project-pages/unit-costs/) from 2022-23, adjusted for inflation

## Primary care

Primary care acitvity is estimated from patient-level data extracted from GP patient systems.

### Primary care telephone/video appointment

[PSSRU Unit costs of social care](https://www.pssru.ac.uk/project-pages/unit-costs/) from 2022-23, adjusted for inflation

### Primary care face to face appointment

[PSSRU Unit costs of social care](https://www.pssru.ac.uk/project-pages/unit-costs/) from 2022-23, adjusted for inflation

### Primary care written appointment

Assumed to be the same as a telephone/video appointment.

## CSDS 

Community activity is estimated using the [community services dataset (CSDS)](https://digital.nhs.uk/data-and-information/data-collections-and-data-sets/data-sets/community-services-data-set).

### Community care contact

[2021-22 PLICS data](https://digital.nhs.uk/data-and-information/publications/statistical/patient-level-activity-and-costing/2021-22), adjusted for inflation.

## CLD

Adult social care activity is estimated using [adult social care client level data (CLD)](https://digital.nhs.uk/data-and-information/data-collections-and-data-sets/data-sets/adult-social-care-client-level-data).

### Adult social care review

[2021-22 PLICS data](https://digital.nhs.uk/data-and-information/publications/statistical/patient-level-activity-and-costing/2021-22), adjusted for inflation.

Assumed 1 hour of social worker time as a proxy cost.

### Adult social care request

[2021-22 PLICS data](https://digital.nhs.uk/data-and-information/publications/statistical/patient-level-activity-and-costing/2021-22), adjusted for inflation.

Assumed 1 hour of social worker time as a proxy cost.

### Adult social care assessment

[2021-22 PLICS data](https://digital.nhs.uk/data-and-information/publications/statistical/patient-level-activity-and-costing/2021-22), adjusted for inflation.

Assumed 1 hour of social worker time as a proxy cost.

### Adult social care carer support

[NHSE adult social care activity and finance report 2022-23](https://digital.nhs.uk/data-and-information/publications/statistical/adult-social-care-activity-and-finance-report/2022-23), adjusted for inflation.

We used the total cost of social support to carers (table 46) and the number of carers (table 49) to estimate a unit cost per carer. We then assumed an average duration of support of 28 days to estimate a cost per day.

### Adult social care long-term support: community

[NHSE adult social care activity and finance report 2022-23](https://digital.nhs.uk/data-and-information/publications/statistical/adult-social-care-activity-and-finance-report/2022-23), adjusted for inflation.

We used the total number of clients receiving long-term care (table 41) and estimated the number receiving support at home by subtracting the numbers in nursing homes and residential homes from the total. We estimated the total cost of support at home using the same methodology (yearly costs, Table 17). We estimated  a unit cost per dat by dividing the yearly cost by the number of patients and by 365.

### Adult social care long-term support: residential home

[NHSE adult social care activity and finance report 2022-23](https://digital.nhs.uk/data-and-information/publications/statistical/adult-social-care-activity-and-finance-report/2022-23), adjusted for inflation.

### Adult social care long-term support: nursing home

[NHSE adult social care activity and finance report 2022-23](https://digital.nhs.uk/data-and-information/publications/statistical/adult-social-care-activity-and-finance-report/2022-23), adjusted for inflation.

### Adult social care short-term support

[NHSE adult social care activity and finance report 2022-23](https://digital.nhs.uk/data-and-information/publications/statistical/adult-social-care-activity-and-finance-report/2022-23), adjusted for inflation.

We used the number of completed ST max episodes (table 28) and gross expenditure (table 29) to calculate a unit cost per episode. We assumed an average episode duration of 28 days to estimate a unit cost per day.