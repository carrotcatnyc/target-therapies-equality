# Preliminary cBioPortal Analysis: EGFR in Lung Adenocarcinoma

## Question for this first analysis

For lung adenocarcinoma (LUAD), how often is **EGFR** altered in two cBioPortal datasets, and what does that suggest about targeted therapy opportunity and dataset representation?

## Why EGFR?

EGFR is a strong first gene for this AP Biology project because it is a well-known lung adenocarcinoma driver gene and has established targeted therapy relevance. It connects clearly to mutation biology, targeted therapy, and fairness in access to biomarker testing.

## Data sources used

Data were queried from cBioPortal public API on May 7, 2026.

| Dataset | cBioPortal study ID | Description |
|---|---|---|
| TCGA LUAD PanCancer Atlas | `luad_tcga_pan_can_atlas_2018` | Public research cohort |
| MSK LUAD 2020 | `luad_mskcc_2020` | MSK-IMPACT clinical sequencing cohort |

## Main results

| Dataset | Sequenced LUAD samples | EGFR-altered samples | EGFR alteration frequency |
|---|---:|---:|---:|
| TCGA LUAD PanCancer Atlas | 566 | 70 | 12.4% |
| MSK LUAD 2020 | 604 | 182 | 30.1% |

## Common EGFR protein changes

| Dataset | Most common EGFR protein changes |
|---|---|
| TCGA LUAD PanCancer Atlas | L858R, E746_A750del, L861Q, E709_T710delinsD, S768I, T790M, G719A |
| MSK LUAD 2020 | L858R, E746_A750del, L747_P753delinsS, L747_A750delinsP, L747_T751del, A767_V769dup, S768I, G719A |

## Demographic notes from available cBioPortal clinical fields

TCGA had race, ethnicity, and sex fields available. MSK LUAD 2020 had sex available, but race/ethnicity was not available in the same simple cBioPortal clinical fields checked here.

### TCGA LUAD race representation

| Race category | All TCGA LUAD patients | EGFR-altered patients |
|---|---:|---:|
| White | 388 | 49 |
| Black or African American | 52 | 6 |
| Asian | 8 | 3 |
| American Indian or Alaska Native | 1 | 0 |
| Unknown | 117 | 12 |

Important caution: the Asian and American Indian/Alaska Native groups are very small in this dataset, so percentages for those groups would be unstable and should not be overinterpreted.

### TCGA LUAD sex representation

| Sex | All TCGA LUAD patients | EGFR-altered patients |
|---|---:|---:|
| Female | 275 | 45 |
| Male | 239 | 21 |
| Unknown | 52 | 4 |

### MSK LUAD 2020 sex representation

| Sex | All MSK LUAD patients | EGFR-altered patients |
|---|---:|---:|
| Female | 402 | 139 |
| Male | 202 | 43 |

## Preliminary interpretation

EGFR alterations appeared in both datasets, but the frequency differed a lot:

- TCGA LUAD: **12.4%** EGFR-altered
- MSK LUAD 2020: **30.1%** EGFR-altered

This does not automatically mean one dataset is “right” and the other is “wrong.” The difference may reflect how the cohorts were collected. TCGA is a public research cohort, while MSK-IMPACT is a clinical sequencing cohort from a major cancer center. Patients who receive clinical sequencing at a specialized center may not represent all lung adenocarcinoma patients.

For the equity question, this is useful because it shows why dataset representation matters. If targeted therapy decisions and research conclusions depend on who is included in genomic datasets, then underrepresented groups may benefit less from precision medicine.

## Equity connection

This preliminary EGFR result supports the project’s social justice focus:

- **Identity:** lung adenocarcinoma patients are affected, especially patients who may not have easy access to genomic testing.
- **Diversity:** datasets may not represent all racial/ethnic, geographic, or socioeconomic groups equally.
- **Justice:** targeted therapy opportunities are unfair if some patients are less likely to be tested or represented in the evidence base.
- **Action:** improving access to biomarker testing and increasing diverse representation in cancer datasets could make precision oncology more equitable.

## Limitations

- This is a preliminary analysis of one gene only.
- cBioPortal clinical demographic fields are incomplete in some studies.
- The MSK dataset used here does not provide the same race/ethnicity fields checked in TCGA.
- The project should avoid making strong claims about race-specific EGFR frequency from very small groups.
- The result shows patterns and raises equity questions; it does not prove unequal access by itself.

## Next steps

1. Repeat the same simple analysis for **ALK** and **KRAS**.
2. Create one bar chart comparing EGFR, ALK, and KRAS alteration frequencies in TCGA vs MSK.
3. Use OncoKB to connect EGFR alterations to Level 1 / Level 2 therapy evidence.
4. In the report, discuss how missing demographic data is itself an equity issue because it limits the ability to evaluate fairness.
