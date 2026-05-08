# Targeted Therapies Equality Project

## Project title

**Equity in Targeted Therapy Opportunities for Lung Adenocarcinoma Patients**

## Guiding scientific question

**Do different populations of lung adenocarcinoma patients have equal representation in genomic datasets and equal access to biomarker-matched targeted therapy opportunities, based on actionable alterations found in TCGA and MSK-IMPACT and therapy evidence from FDA drug labels, NCCN guidelines, and clinical trials?**

Simpler version for a presentation board:

**Are targeted therapy opportunities for lung adenocarcinoma equally available across different patient populations?**

## Why this matters

Targeted therapies can greatly improve outcomes for some lung adenocarcinoma patients, but patients only benefit if they have access to genomic testing, accurate biomarker interpretation, appropriate drugs, and clinical trials. If some populations are underrepresented in genomic datasets, clinical trials, or guideline evidence, precision oncology may unintentionally widen existing health disparities.

This project addresses fairness, access, health equity, and positive social impact by studying whether the evidence and opportunities behind targeted cancer treatment are distributed equitably.

## Cancer type

**Lung adenocarcinoma (LUAD)**

Lung adenocarcinoma is a good focus because it has several well-established actionable biomarkers and targeted therapies.

## Candidate biomarkers / genes

Initial genes and alterations to investigate:

- **EGFR**
- **ALK**
- **ROS1**
- **BRAF**
- **MET**
- **RET**
- **NTRK1 / NTRK2 / NTRK3**
- **ERBB2 / HER2**
- **KRAS**

These can be refined using OncoKB evidence levels and available cBioPortal data.

## Core data sources

### 1. TCGA via cBioPortal

- Source: <https://www.cbioportal.org/>
- Dataset example: TCGA Lung Adenocarcinoma / LUAD
- Role in project: public research cohort for lung adenocarcinoma genomics and clinical-demographic variables.
- Data to collect:
  - Number of LUAD patients
  - Race/ethnicity, sex, age, and other available clinical variables
  - Frequency of actionable alterations
  - Differences in mutation frequency by demographic group, if sample size allows

### 2. MSK-IMPACT via cBioPortal

- Source: <https://www.cbioportal.org/>
- Dataset example: MSK-IMPACT clinical sequencing cohorts that include lung adenocarcinoma
- Role in project: real-world clinical sequencing comparison cohort.
- Data to collect:
  - Number of LUAD patients sequenced
  - Demographic variables where available
  - Frequency of actionable alterations
  - Comparison with TCGA to assess whether research and clinical cohorts look similar or different

### 3. ClinicalTrials.gov

- Source: <https://clinicaltrials.gov/>
- Role in project: trial access and availability for targeted therapy opportunities.
- Data to collect:
  - Number of LUAD targeted therapy trials for selected biomarkers
  - Trial status: recruiting, active, completed
  - Trial locations by state/country/region
  - Eligibility requirements involving biomarkers
  - Whether trials appear geographically concentrated

### 4. FDA drug labels via OncoKB Level 1

- Source: <https://www.oncokb.org/>
- Role in project: identifies biomarkers with FDA-recognized therapeutic evidence.
- Data to collect:
  - LUAD biomarkers with OncoKB Level 1 evidence
  - Matched targeted therapies
  - Biomarker-drug-cancer type combinations

### 5. NCCN-supported evidence via OncoKB Level 2

- Source: <https://www.oncokb.org/>
- Role in project: identifies biomarkers with standard-care or guideline-supported therapeutic relevance beyond FDA label evidence.
- Data to collect:
  - LUAD biomarkers with OncoKB Level 2 evidence
  - Matched targeted therapies or guideline-supported options
  - Differences between FDA-labeled and NCCN-supported therapy opportunities

## Proposed analysis plan

### Step 1: Define actionable biomarkers

Use OncoKB to define LUAD-relevant actionable biomarkers:

- Level 1: FDA-recognized biomarkers and therapies
- Level 2: NCCN or standard-care supported biomarkers and therapies

Create a table with:

- Gene
- Alteration type
- Therapy
- OncoKB evidence level
- FDA label or NCCN support

### Step 2: Query TCGA LUAD in cBioPortal

For the selected biomarkers:

- Count total LUAD cases
- Count cases with each actionable alteration
- Calculate alteration frequency overall
- Stratify by available demographic variables, such as race/ethnicity, sex, and age group

Potential output:

- Bar chart of actionable alteration frequency by gene
- Table of alteration frequency by demographic group
- Short note on missing or limited demographic data

### Step 3: Query MSK-IMPACT LUAD in cBioPortal

Repeat the same analysis for MSK-IMPACT LUAD cases:

- Count total LUAD cases
- Count actionable alterations
- Compare alteration frequencies with TCGA
- Compare available demographic representation with TCGA

Potential output:

- TCGA vs MSK-IMPACT comparison chart
- Discussion of how research cohorts and clinical sequencing cohorts may differ

### Step 4: Assess clinical trial access

Use ClinicalTrials.gov to search for lung adenocarcinoma targeted therapy trials involving the selected biomarkers.

Suggested search terms:

- `lung adenocarcinoma EGFR targeted therapy`
- `lung adenocarcinoma ALK inhibitor`
- `lung adenocarcinoma ROS1 targeted therapy`
- `lung adenocarcinoma RET inhibitor`
- `lung adenocarcinoma MET exon 14`
- `lung adenocarcinoma KRAS G12C inhibitor`

For each trial or group of trials, collect:

- Trial title
- Biomarker/gene
- Therapy type
- Recruitment status
- Locations
- Eligibility criteria

Potential output:

- Map or table of trial locations
- Count of trials by biomarker
- Discussion of geographic access barriers

### Step 5: Compare therapy evidence with actual opportunity

Combine the data sources to ask:

- Which biomarkers have FDA label support?
- Which biomarkers have NCCN-supported evidence?
- Which biomarkers are found in TCGA/MSK-IMPACT patients?
- Are patients from different groups equally represented in the datasets used to study these biomarkers?
- Are trials for these biomarkers broadly available, or concentrated in certain locations?

### Step 6: Equity interpretation

Discuss whether precision oncology opportunities may be unequal because of:

- Underrepresentation in genomic datasets
- Unequal access to tumor genomic testing
- Unequal access to academic cancer centers
- Unequal access to clinical trials
- Insurance or cost barriers
- Geographic distance from trial sites
- Missing or incomplete demographic data

## Possible final products

- A written report
- A slide deck or science fair board
- Tables of actionable biomarkers and evidence levels
- Charts comparing TCGA and MSK-IMPACT alteration frequencies
- A clinical trial access table or map
- A short equity-focused conclusion with recommendations

## Possible hypothesis

**Lung adenocarcinoma targeted therapy opportunities are not equally distributed across patient populations because genomic datasets, biomarker testing, and clinical trial access may underrepresent or underserve some demographic and geographic groups.**

## Limitations to acknowledge

- TCGA is a research dataset and may not represent all real-world cancer patients.
- MSK-IMPACT reflects patients treated or sequenced in a major cancer-center context and may also have selection bias.
- Some cBioPortal studies have incomplete race, ethnicity, or socioeconomic data.
- ClinicalTrials.gov shows trial availability but does not always provide complete participant demographic enrollment data.
- OncoKB evidence levels identify therapy evidence but do not directly measure whether patients can actually access the therapy.

## Equity and social impact connection

This project can help show that precision medicine is not only a scientific issue but also a fairness issue. If targeted therapies depend on who gets tested, who is represented in datasets, and who can reach clinical trials, then improving equity in cancer care requires better access to genomic testing, more diverse research participation, and broader availability of biomarker-matched therapies.
