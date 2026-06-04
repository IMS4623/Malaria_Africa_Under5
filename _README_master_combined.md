# README — africa_master_combined.csv

The combined file currently has **8,326 rows** and **74 columns**, covers **54 African countries**, and spans years **1871 to 2100**.

## Key structure

- **Unit of observation:** country-year
- **Primary keys:** `country_iso3`, `year`
- **Country name column:** `country_name`
- Missing values mean the source did not provide a value for that country-year

## Column dictionary

| Column | Meaning | Unit / scale | Typical values / notes | Non-null rows |
|---|---|---|---|---|
| `country_iso3` | ISO 3166-1 alpha-3 country code for the country. | Text code | Examples: DZA, NGA, KEN. | 8,326 |
| `country_name` | Canonical country name used in the merged master file. | Text | Examples: Algeria, Nigeria, Kenya. | 8,326 |
| `year` | Calendar year of the observation. | Integer year | Overall file spans 1871 to 2100. | 8,326 |
| `children_under_5_total__number_of_children_under_5` | Observed estimate of the total number of children younger than 5 years. | Number of children | Raw count. Missing where only projected series was available. | 3,996 |
| `children_under_5_total__number_of_children_under_5_projected` | Projected estimate of the total number of children younger than 5 years. | Number of children | Projection-based count from OWID series. | 4,158 |
| `stunting_prevalence_under5_pct` | Share of children under 5 who are stunted. | Percent (%) | Typically 0–100. | 1,350 |
| `anemia_prevalence_under5_pct` | Share of children under 5 with anemia. | Percent (%) | Typically 0–100. | 1,080 |
| `preprimary_net_enrollment_pct` | Net enrollment rate in pre-primary education. | Percent (%) | Usually interpreted as percent of official pre-primary age group enrolled in pre-primary school. | 551 |
| `vaccination_measles_first_dose_mcv1` | Coverage of the first measles-containing vaccine dose (MCV1). | Percent coverage (%) | Usually 0–100. | 2,235 |
| `vaccination_hepatitis_b_hepb3` | Coverage of the third hepatitis B vaccine dose (HepB3). | Percent coverage (%) | Usually 0–100. | 1,169 |
| `vaccination_diphtheria_tetanus_pertussis_dtp3` | Coverage of the third diphtheria-tetanus-pertussis vaccine dose (DTP3). | Percent coverage (%) | Usually 0–100. | 2,243 |
| `vaccination_inactivated_polio_ipv1` | Coverage of the first inactivated polio vaccine dose (IPV1). | Percent coverage (%) | Usually 0–100. | 478 |
| `vaccination_polio_pol3` | Coverage of the third polio vaccine dose (POL3). | Percent coverage (%) | Usually 0–100. | 2,245 |
| `vaccination_h_influenzae_type_b_hib3` | Coverage of the third Haemophilus influenzae type b vaccine dose (Hib3). | Percent coverage (%) | Usually 0–100. | 937 |
| `vaccination_rubella_rcv1` | Coverage of the first rubella-containing vaccine dose (RCV1). | Percent coverage (%) | Usually 0–100. | 403 |
| `vaccination_pneumococcal_conjugate_pcv3` | Coverage of the third pneumococcal conjugate vaccine dose (PCV3). | Percent coverage (%) | Usually 0–100. | 537 |
| `vaccination_rotavirus_rotac` | Coverage of the full recommended rotavirus vaccine course (RotaC, chart-specific label). | Percent coverage (%) | Usually 0–100. | 440 |
| `exclusive_breastfeeding_pct` | Share of infants exclusively breastfed. | Percent (%) | Typically measured among infants under 6 months; chart definition should be checked if used in a paper. | 320 |
| `child_mortality_deaths_per_100_live_births` | Child mortality rate from the OWID child mortality series. | Deaths per 100 live births | Under-5 mortality style measure. | 3,749 |
| `low_birthweight_pct` | Share of babies born with low birthweight. | Percent (%) | Typically birthweight under 2,500 g. | 798 |
| `stillbirths_per_100_births` | Stillbirth rate. | Stillbirths per 100 births | Rate scaled per 100 births in this master file. | 1,296 |
| `gdp_constant_2015_usd` | Gross domestic product in constant 2015 US dollars. | Constant 2015 US$ | Level, not per capita. | 3,151 |
| `gdp_per_capita_ppp_constant_2021_intl_usd` | GDP per capita adjusted for purchasing power parity. | Constant 2021 international $ (PPP) | Per-person economic output. | 1,796 |
| `human_development_index` | Human Development Index composite score. | Index (0–1) | Higher values indicate higher human development. | 1,597 |
| `household_type_couple_with_children` | Share of households classified as couple with children. | Share / fraction of households | Chart-derived household composition category. May be stored as fraction or percent depending on source export; verify before presenting as percent. | 289 |
| `household_type_single_parent_with_children` | Share of households classified as single parent with children. | Share / fraction of households | Chart-derived household composition category. | 289 |
| `household_type_couple` | Share of households classified as couple without children. | Share / fraction of households | Chart-derived household composition category. | 289 |
| `household_type_one_person` | Share of one-person households. | Share / fraction of households | Chart-derived household composition category. | 289 |
| `household_type_extended_family` | Share of households classified as extended family. | Share / fraction of households | Chart-derived household composition category. | 289 |
| `household_type_non_relatives` | Share of households composed of non-relatives. | Share / fraction of households | Chart-derived household composition category. | 289 |
| `household_type_unknown` | Share of households in unknown / other category. | Share / fraction of households | Residual or unclassified category. | 288 |
| `daily_median_income_ppp_2021_intl_usd` | Daily median income or consumption. | 2021 international $ PPP per person per day | Comparable cross-country income/consumption measure. | 269 |
| `sex_ratio_at_birth_males_per_100_females` | Sex ratio at birth. | Male births per 100 female births | Biological ratio measure. | 3,996 |
| `malaria_incidence_rate` | Malaria incidence rate among children under 5 from GBD. | Rate per 100,000 population | Point estimate. | 1,836 |
| `malaria_incidence_rate_lower` | Lower uncertainty bound for malaria incidence rate. | Rate per 100,000 population | GBD lower bound. | 1,836 |
| `malaria_incidence_rate_upper` | Upper uncertainty bound for malaria incidence rate. | Rate per 100,000 population | GBD upper bound. | 1,836 |
| `malaria_prevalence_rate` | Malaria prevalence rate among children under 5 from GBD. | Rate per 100,000 population | Point estimate. | 1,836 |
| `malaria_prevalence_rate_lower` | Lower uncertainty bound for malaria prevalence rate. | Rate per 100,000 population | GBD lower bound. | 1,836 |
| `malaria_prevalence_rate_upper` | Upper uncertainty bound for malaria prevalence rate. | Rate per 100,000 population | GBD upper bound. | 1,836 |
| `all_cause_under5_mortality_rate` | All-cause mortality rate among children under 5 from GBD. | Rate per 100,000 population | Point estimate. This is not malaria-specific mortality. | 1,836 |
| `all_cause_under5_mortality_rate_lower` | Lower uncertainty bound for all-cause under-5 mortality rate. | Rate per 100,000 population | GBD lower bound. | 1,836 |
| `all_cause_under5_mortality_rate_upper` | Upper uncertainty bound for all-cause under-5 mortality rate. | Rate per 100,000 population | GBD upper bound. | 1,836 |
| `acute_hepatitis_b_incidence_rate` | Incidence rate of acute hepatitis B in children under 5 from GBD. | Rate per 100,000 population | Point estimate. | 1,836 |
| `acute_hepatitis_b_incidence_rate_lower` | Lower uncertainty bound for acute hepatitis B incidence rate. | Rate per 100,000 population | GBD lower bound. | 1,836 |
| `acute_hepatitis_b_incidence_rate_upper` | Upper uncertainty bound for acute hepatitis B incidence rate. | Rate per 100,000 population | GBD upper bound. | 1,836 |
| `acute_hepatitis_c_incidence_rate` | Incidence rate of acute hepatitis C in children under 5 from GBD. | Rate per 100,000 population | Point estimate. | 1,836 |
| `acute_hepatitis_c_incidence_rate_lower` | Lower uncertainty bound for acute hepatitis C incidence rate. | Rate per 100,000 population | GBD lower bound. | 1,836 |
| `acute_hepatitis_c_incidence_rate_upper` | Upper uncertainty bound for acute hepatitis C incidence rate. | Rate per 100,000 population | GBD upper bound. | 1,836 |
| `diarrheal_diseases_incidence_rate` | Incidence rate of diarrheal diseases in children under 5 from GBD. | Rate per 100,000 population | Point estimate. | 1,836 |
| `diarrheal_diseases_incidence_rate_lower` | Lower uncertainty bound for diarrheal diseases incidence rate. | Rate per 100,000 population | GBD lower bound. | 1,836 |
| `diarrheal_diseases_incidence_rate_upper` | Upper uncertainty bound for diarrheal diseases incidence rate. | Rate per 100,000 population | GBD upper bound. | 1,836 |
| `neonatal_encephalopathy_due_to_birth_asphyxia_and_trauma_incidence_rate` | Incidence rate of neonatal encephalopathy due to birth asphyxia and trauma. | Rate per 100,000 population | Point estimate from GBD. | 1,836 |
| `neonatal_encephalopathy_due_to_birth_asphyxia_and_trauma_incidence_rate_lower` | Lower uncertainty bound for neonatal encephalopathy due to birth asphyxia and trauma incidence rate. | Rate per 100,000 population | GBD lower bound. | 1,836 |
| `neonatal_encephalopathy_due_to_birth_asphyxia_and_trauma_incidence_rate_upper` | Upper uncertainty bound for neonatal encephalopathy due to birth asphyxia and trauma incidence rate. | Rate per 100,000 population | GBD upper bound. | 1,836 |
| `neonatal_preterm_birth_incidence_rate` | Incidence rate of neonatal preterm birth condition from GBD. | Rate per 100,000 population | Point estimate. | 1,836 |
| `neonatal_preterm_birth_incidence_rate_lower` | Lower uncertainty bound for neonatal preterm birth incidence rate. | Rate per 100,000 population | GBD lower bound. | 1,836 |
| `neonatal_preterm_birth_incidence_rate_upper` | Upper uncertainty bound for neonatal preterm birth incidence rate. | Rate per 100,000 population | GBD upper bound. | 1,836 |
| `neonatal_sepsis_and_other_neonatal_infections_incidence_rate` | Incidence rate of neonatal sepsis and other neonatal infections. | Rate per 100,000 population | Point estimate from GBD. | 1,836 |
| `neonatal_sepsis_and_other_neonatal_infections_incidence_rate_lower` | Lower uncertainty bound for neonatal sepsis and other neonatal infections incidence rate. | Rate per 100,000 population | GBD lower bound. | 1,836 |
| `neonatal_sepsis_and_other_neonatal_infections_incidence_rate_upper` | Upper uncertainty bound for neonatal sepsis and other neonatal infections incidence rate. | Rate per 100,000 population | GBD upper bound. | 1,836 |
| `nutritional_deficiencies_incidence_rate` | Incidence rate of nutritional deficiencies in children under 5 from GBD. | Rate per 100,000 population | Point estimate. | 1,836 |
| `nutritional_deficiencies_incidence_rate_lower` | Lower uncertainty bound for nutritional deficiencies incidence rate. | Rate per 100,000 population | GBD lower bound. | 1,836 |
| `nutritional_deficiencies_incidence_rate_upper` | Upper uncertainty bound for nutritional deficiencies incidence rate. | Rate per 100,000 population | GBD upper bound. | 1,836 |
| `temp_mean_c` | Mean air temperature for the year. | Degrees Celsius (°C) | Climate variable from the prior raw master file. | 1,092 |
| `temp_max_c` | Maximum air temperature for the year. | Degrees Celsius (°C) | Climate variable from the prior raw master file. | 1,092 |
| `temp_min_c` | Minimum air temperature for the year. | Degrees Celsius (°C) | Climate variable from the prior raw master file. | 1,092 |
| `rel_humidity_pct` | Relative humidity. | Percent (%) | Climate variable. | 1,092 |
| `rain_mm_per_day` | Average rainfall per day. | Millimeters per day (mm/day) | Climate variable. | 1,092 |
| `rain_mm_year` | Total rainfall over the year. | Millimeters per year (mm/year) | Climate variable. | 1,092 |
| `female_primary_gross_enrol` | Female gross enrollment ratio in primary education. | Percent (%) | Education variable from the prior raw master file. | 830 |
| `female_secondary_gross_enrol` | Female gross enrollment ratio in secondary education. | Percent (%) | Education variable from the prior raw master file. | 597 |
| `female_tertiary_gross_enrol` | Female gross enrollment ratio in tertiary education. | Percent (%) | Education variable from the prior raw master file. | 566 |
| `female_primary_completion_rate` | Female primary completion rate. | Percent (%) | Education variable from the prior raw master file. | 683 |
| `malaria_prev_rate_female_per_100k` | Female malaria prevalence rate from the prior raw master file. | Rate per 100,000 female population | Retained raw variable from earlier filtered dataset. | 1,029 |

## Column groups

### 1) Identifiers
- `country_iso3`, `country_name`, `year`

### 2) Demography and nutrition
- under-5 population, stunting, anemia, breastfeeding, low birthweight, stillbirths

### 3) Education and immunization
- pre-primary enrollment, female education variables, vaccine coverage variables

### 4) Economic and development context
- GDP, GDP per capita, HDI, daily median income, household composition

### 5) Malaria and child-health burden from GBD
- malaria incidence/prevalence, all-cause under-5 mortality, hepatitis B/C, diarrheal diseases, neonatal and nutritional conditions, each with uncertainty bounds

### 6) Climate
- temperature, humidity, rainfall

## How to interpret the uncertainty columns

For GBD-based variables, each main point estimate is accompanied by two additional columns:
- `_lower`: lower uncertainty bound
- `_upper`: upper uncertainty bound

Example:
- `malaria_incidence_rate` = point estimate
- `malaria_incidence_rate_lower` = lower bound
- `malaria_incidence_rate_upper` = upper bound


## File provenance summary

- OWID-derived variables: population under 5, stunting, anemia, pre-primary enrollment, vaccine coverage, exclusive breastfeeding, child mortality, low birthweight, stillbirths, GDP, GDP per capita, HDI, household composition, daily median income, sex ratio at birth.
- GBD-derived variables: malaria incidence and prevalence, all-cause under-5 mortality, hepatitis B, hepatitis C, diarrheal diseases, neonatal encephalopathy, neonatal preterm birth, neonatal sepsis/other neonatal infections, nutritional deficiencies.
- Previously study master variables: climate(NASA Power), female education (OWID), female malaria prevalence (IHME).

- Rows: **8,326**
- Columns: **74**
- Unique countries: **54**
- Year range: **1871–2100**
