# Harris County Overdose Burden: Initial Numbers

**Status:** preliminary extraction for the research outline

**Retrieved:** 2026-09-15

## Source and definitions

The numbers below come from the Harris County Public Health (HCPH) Substance Use Data Hub, whose death-page disclaimer says the fatal-overdose data come from the Harris County Institute of Forensic Sciences (HCIFS). The public dashboard is available at <https://od2a-substance-use-surveillance-hcpublichealth.hub.arcgis.com/pages/deaths>.

The five-year comparison is the public HCPH ArcGIS dashboard view titled **Substance-Involved Deaths in Harris County, Texas, and the United States, 2021-2025**: <https://experience.arcgis.com/experience/ec175d8e51174c97b6fdea33da438a51/page/Graph?views=IFS-5-Year-Comparison>. It reports Harris County totals of 1,159 (2021), 1,177 (2022), 1,126 (2023), 970 (2024), and 776 (2025).

Fentanyl counts come from the dashboard's public ArcGIS FeatureServer table, **IFS CDC Drug Group**: <https://services3.arcgis.com/FsUrhUGHe9VfghT8/arcgis/rest/services/IFS_CDC_Drug_Group/FeatureServer/0/query?where=1%3D1%26outFields=*%26returnGeometry=false%26f=pjson>. The table identifies `death_year`, `substance_group`, and `counts`; the fentanyl rows are 482 (2021), 583 (2022), 570 (2023), 395 (2024), and 219 (2025).

HCPH warns that reporting can be delayed by pending toxicology and that IFS substance fields are free text, creating possible spelling differences, classification differences, duplication, and misclassification. These recent years should therefore be labeled as HCPH/HCIFS aggregate surveillance values, not treated as final national mortality estimates.

## Mortality trend

| Year | HCPH substance-involved deaths | Change from prior year | Change from 2021 |
|---:|---:|---:|---:|
| 2021 | 1,159 | -- | 0.0% |
| 2022 | 1,177 | +1.6% | +1.6% |
| 2023 | 1,126 | -4.3% | -2.8% |
| 2024 | 970 | -13.9% | -16.3% |
| 2025 | 776 | -20.0% | -33.0% |

The five-year trend is a **33.0% decrease from 2021 to 2025**, although the series peaked at 1,177 deaths in 2022. The 2025 value is 34.1% below the 2022 peak. The dashboard's own caveats about delayed toxicology and recent-year reporting should accompany any use of the 2025 value.

## Fentanyl contribution

| Year | HCPH/HCIFS fentanyl-involved deaths | All HCPH substance-involved deaths | Fentanyl share of all substance-involved deaths |
|---:|---:|---:|---:|
| 2021 | 482 | 1,159 | 41.6% |
| 2022 | 583 | 1,177 | 49.5% |
| 2023 | 570 | 1,126 | 50.6% |
| 2024 | 395 | 970 | 40.7% |
| 2025 | 219 | 776 | 28.2% |

The share is calculated as `fentanyl-involved deaths / all substance-involved deaths` for the same HCPH year. Drug categories can overlap, so fentanyl counts must not be added to opioid, stimulant, cocaine, or other category counts. The apparent fall in the 2025 fentanyl share should be treated cautiously because the dashboard states that toxicology reporting can lag.

## Polysubstance share

A Harris County polysubstance share is **not yet computable from the public products located**. The public HCPH dashboard and its exposed `IFS_CDC_Drug_Group` table provide substance-category counts, but they do not expose the number of distinct substances per death or a mutually exclusive single-substance versus multiple-substance field. Adding category totals would be invalid because categories overlap.

The Texas DSHS publication **Polysubstance-related Poisoning Deaths in Texas, 2012-2022** is a statewide source, not a verified Harris County estimate, so it should not be substituted for the requested local share. A local polysubstance percentage requires either:

1. a de-identified HCIFS/HCPH aggregate with a documented polysubstance definition; or
2. case-level substance fields that can be legally and ethically processed under an approved data-use arrangement.

Until then, report polysubstance share as a data gap rather than infer it from the fentanyl, opioid, stimulant, cocaine, and benzodiazepine series.

## Rough outline for Section 4: City Profile and Harm Reduction Landscape

1. **Data source and scope:** HCPH Substance Use Data Hub, sourced from HCIFS, with the dashboard's definitions and toxicology/reporting caveats.
2. **Trend:** 1,159 deaths in 2021, a peak of 1,177 in 2022, and 776 in 2025, a 33.0% decrease from 2021 to 2025.
3. **Fentanyl:** 482 to 583 to 570 to 395 to 219 deaths from 2021-2025; the corresponding share of all substance-involved deaths ranges from 28.2% to 50.6%.
4. **Polysubstance:** local share not computable from the public aggregate layer; do not add overlapping drug categories.
5. **Non-fatal burden:** add HCPH ESSENCE, EMS, hospital, or other published non-fatal volume if the source definition and window can be verified; otherwise document the absence.
6. **Demographics with consequences:** connect population, racial/ethnic composition, poverty, and uninsurance to likely naloxone, treatment, transportation, or medication-access barriers; do not report them as bare descriptors.
7. **Treatment and infectious disease:** assess treatment capacity and retention, then HIV and hepatitis C burden as injection-drug-use proxies, with source windows and geographic limits.
8. **Criminal justice:** explain how possession enforcement, incarceration, reentry, and emergency contact concerns may change treatment-seeking and overdose-response behavior in Houston.
9. **Existing infrastructure:** name organizations and assess what each actually does, whom it reaches, and which geographies it covers; this must be an assessment, not a directory.
10. **Who is missed:** identify populations current outreach is unlikely to reach and the mechanism of exclusion, including people who do not self-identify as drug users.
11. **Single critical gap:** end with one sentence naming the most consequential structural gap in Houston's harm-reduction system, supported by the preceding evidence.
12. **Interpretation rule:** every paragraph must state a local condition, give evidence and its time window, interpret it, and draw an implication for harm-reduction access or delivery. Describe the recent mortality decline cautiously because late toxicology and free-text classification may affect the newest observations; validate or sensitivity-check against Texas DSHS death-certificate measures.

## Reproducibility note

The aggregate values are safe to report in this memo because they contain no person-level records, addresses, case numbers, or exact locations. Before manuscript use, rerun the public dashboard/API query, record the retrieval date and source-table modification date, and preserve the exact query response or a derived aggregate table with the source citation.
