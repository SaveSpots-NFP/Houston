# Harris County Overdose Data Availability Audit

**Checked:** 2026-09-15

## Bottom line

Harris County does not appear to publish a downloadable, case-level overdose-death or toxicology dataset through the Harris County Institute of Forensic Sciences (HCIFS) website. The county does publish public aggregate products through Harris County Public Health (HCPH), and HCIFS exposes a limited case-status lookup. HCIFS also accepts individual autopsy-report requests and Texas Public Information Act requests by email. The available evidence supports treating Houston as **Environment B**: aggregate public data are available, but case-level mortality analysis requires a separate data request, data-use arrangement, or a successful public-information response.

This is a documented absence, not a claim that the records do not exist.

### Provisional environment declaration

Houston/Harris County appears to fit **Environment B**, with a request-based hybrid: public aggregate mortality data are available, but case-level Medical Examiner records are not openly published. This judgment is supported by searches of the Harris County Institute of Forensic Sciences website, including its Case Status, autopsy-report, and Media Relations/Public Information pages; the Harris County Public Health Substance Use Data Hub; the Texas DSHS Drug-Related Deaths dashboard; CDC/NCHS mortality products; and the relevant public data portals. Those searches found aggregate death trends, county/ZIP-level public visualizations, and limited recent case lookup, but no downloadable HCIFS overdose case file or toxicology dataset. HCIFS instead directs report and Texas Public Information Act requests through email, so the project can proceed with aggregate data while treating case-level mortality as a possible future request rather than an assumed input.

## Source audit

### 1. Harris County Institute of Forensic Sciences: public website

Source: <https://ifs.harriscountytx.gov/>

- The site has no obvious public overdose-death dashboard, downloadable overdose-death table, public toxicology file, or open case-level mortality extract.
- The site has a **Case Status** tool: <https://ifs.harriscountytx.gov/Learning-Center/Case-Status>.
- Case Status permits a case-number search or an advanced search by name, date range, and gender. The site explicitly says the tool provides **basic information** for Medical Examiner cases dating back **24 months**.
- The page states that case-status information is confirmed for media use. It is not described as a bulk data download and does not expose a historical case-level analytic file.
- No account registration is required to view the public site or to use the visible case-status workflow.

Interpretation: this is a limited lookup service, not Environment A case-level access.

### 2. HCIFS autopsy reports

Source: <https://ifs.harriscountytx.gov/family-services/Autopsy-Reports>

- Completed autopsy reports can be requested by email at `ifsadministrativeservices@ifs.hctx.net` or by postal mail.
- The request instructions ask for identifying case details, such as case number, deceased person's name, date of death, and county of death, plus requester contact information.
- An electronic PDF copy is available at no charge when the request is fulfilled; certified printed copies have a per-page fee.
- The page describes individual report requests. It does not offer a public batch download, case-level overdose file, or toxicology table.

Interpretation: individual reports may be obtainable, but this route is not an already-public research dataset and would not by itself support a privacy-preserving countywide analysis without a negotiated aggregation or data-use process.

### 3. HCIFS public-information and data requests

Source: <https://ifs.harriscountytx.gov/newsroom/Media-Relations>

- HCIFS says public-information and data requests must be submitted in writing by email.
- The designated address for Texas Public Information Act requests is `IFSPIO@ifs.hctx.net`.
- The page says the Institute operates under the Texas Public Information Act, Government Code Chapter 552.
- The page does not promise that case-level overdose records, toxicology records, or bulk extracts will be released. Availability would depend on the request, applicable confidentiality provisions, record format, and the Institute's response.

Interpretation: a written request is a viable discovery route, but it is not evidence that the requested case-level data are publicly available. A request should ask first for an aggregate, de-identified extract and should avoid requesting names, addresses, exact locations, or other unnecessary identifiers.

### 4. Harris County Public Health Substance Use Data Hub

Sources:

- Home: <https://od2a-substance-use-surveillance-hcpublichealth.hub.arcgis.com/>
- Deaths page: <https://od2a-substance-use-surveillance-hcpublichealth.hub.arcgis.com/pages/deaths>
- Death trends app embedded in the deaths page: <https://experience.arcgis.com/experience/ec175d8e51174c97b6fdea33da438a51/>

- HCPH publicly states that its Substance Use Data Hub provides fatal and non-fatal overdose information for Harris County.
- The public deaths page displays an interactive breakdown of substance-involved deaths and trend views by age, sex, race, drug type, and five-year comparison.
- The home page describes a public map with age-adjusted rates by Harris County ZIP code and county/state/national comparisons. The home page reports substance-involved deaths for 2021-2025.
- The death-page disclaimer states that HCPH gets fatal-overdose data from HCIFS and that the IFS data include substance-involved deaths for individuals pronounced dead in Harris County.
- The disclaimer says HCPH reports accidental deaths, suicides, homicides, and deaths of undetermined causes.
- The disclaimer warns that reporting can be delayed while toxicology results are pending.
- The disclaimer says IFS substance fields are entered as free text, which can produce inconsistent classifications, misspellings, misclassification, duplication, and naming differences.
- The public hub exposes ArcGIS search/catalog controls and a public catalog export control, but the deaths page itself does not present a downloadable case-level table. No account was needed to view the hub or deaths page. A visible ArcGIS sign-in option is for the broader platform and is not required for the public product.
- The hub provides `od2ainfo@phs.hctx.net` for overdose-related questions or data requests.

Interpretation: HCPH is the strongest local public source found. It provides aggregate, privacy-preserving outputs and methodological caveats, not a public case-level mortality file.

### 5. Texas Department of State Health Services: Texas Health Data

Sources:

- Drugs and Alcohol dashboard index: <https://healthdata.dshs.texas.gov/dashboards/drugs-and-alcohol>
- Drug-related deaths dashboard: <https://healthdata.dshs.texas.gov/dashboard/drugs-and-alcohol/all-drugs/drug-related-deaths>

- The Texas Health Data dashboard publicly provides drug-related death information at state and county levels, including demographic groups and drug categories.
- The dashboard uses Texas Vital Statistics death-certificate data rather than the HCIFS case files directly.
- It describes county of occurrence, county of residence, age, race/ethnicity, sex, year of death, and underlying cause of death.
- It identifies ICD-10 groupings for opioids, heroin, prescription and synthetic opioids, benzodiazepines, cocaine, psychostimulants, cannabis, and other substances.
- Counts of 1-9 are suppressed, and rates with numerators of 1-20 are suppressed. Suppressed spreadsheet values appear as `-1`.
- The dashboard is publicly viewable without an account. It provides a public contact route, `vstat@dshs.texas.gov`, for questions about the data.

Interpretation: this is a usable aggregate alternative for county-level mortality trends, with death-certificate definitions and suppression. It does not provide case-level records or the full toxicology detail available in individual ME files.

### 6. Federal aggregate alternatives

The Texas dashboard itself links to CDC opioid-overdose dashboards. CDC WONDER and related CDC mortality products can support aggregate county-level analyses using death-certificate data, subject to suppression and the product's geography/time limits. These sources are alternatives for Environment B analyses, not substitutes for HCIFS case-level toxicology records.

## 6.1 Inventory table

The table records the datasets and endpoints checked as of 2026-09-15. "Not stated" means the publisher did not expose a clear record vintage on the public landing page; it does not mean the data are current. Fine geographies listed below are the publisher's available resolution, not necessarily the resolution used in the analysis.

| Dataset name and publisher | Endpoint, API identifier, or access route | Actual published resolution | Most recent record date / retrieved | Access | Verdict |
|---|---|---|---|---|---|
| 2020 Census P.L. 94-171 P1 population, U.S. Census Bureau | [2020 redistricting summary files](https://www.census.gov/programs-surveys/decennial-census/about/rdo/summary-files.html); table P1, variable P1_001N | Census block, block group, tract, and larger geographies | 2020 / 2026-09-15 | Open download/API | Use for population denominators and geography validation; do not use as a current population estimate |
| 2020 Census TIGER/Line geography, U.S. Census Bureau | [2020 Census geographic support products](https://www.census.gov/programs-surveys/decennial-census/about/rdo/summary-files.html) | Block, block group, tract, and larger geographies | 2020 boundaries / 2026-09-15 | Open download | Use for boundary and spatial joins; preserve the 2020 vintage |
| ACS 5-year Subject Table S1701 Poverty, U.S. Census Bureau | [2024 ACS subject-table API](https://api.census.gov/data/2024/acs/acs5/subject/groups/S1701.json) | County, tract, and other supported ACS geographies; no block-level estimates | 2020-2024 / 2026-09-15 | Open API/data.census.gov | Use as a modeled/contextual vulnerability layer |
| ACS 5-year Subject Table S2701 Uninsured, U.S. Census Bureau | [2024 ACS subject-table API](https://api.census.gov/data/2024/acs/acs5/subject/groups/S2701.json) | County, tract, and other supported ACS geographies; no block-level estimates | 2020-2024 / 2026-09-15 | Open API/data.census.gov | Use as a modeled/contextual access-barrier layer; do not allocate it to blocks |
| CDC/ATSDR Social Vulnerability Index, CDC/ATSDR | [SVI data and documentation](https://www.atsdr.cdc.gov/place-health/php/svi/svi-data-documentation-download.html) | Census tract and larger geographies | 2022 SVI / 2026-09-15 | Open download | Use as a published vulnerability index with its own geography and vintage; do not treat it as a direct overdose measure |
| Underlying Cause of Death, CDC/NCHS via CDC WONDER | [Underlying Cause of Death 1999-2020](https://wonder.cdc.gov/ucd-icd10.html) | County of residence and larger geographies; queryable by cause, year, demographics, and intent | 2020 final in checked endpoint / 2026-09-15 | Open query with data-use restrictions | Use for historical validation/sensitivity; counts of 9 or fewer may not be published and no identity inference is permitted |
| Drug-related deaths, Texas DSHS Vital Statistics | [Texas Health Data dashboard](https://healthdata.dshs.texas.gov/dashboard/drugs-and-alcohol/all-drugs/drug-related-deaths) | State and county, with demographic breakdowns | Current dashboard release / 2026-09-15 | Open dashboard; contact available | Use as the primary public mortality comparison, subject to suppression and death-certificate definitions |
| Substance-involved deaths, Harris County Public Health | [HCPH Substance Use Data Hub deaths page](https://od2a-substance-use-surveillance-hcpublichealth.hub.arcgis.com/pages/deaths) and embedded mortality app | Harris County and public ZIP-code map; trend views by demographic and drug category | Home page displayed 2021-2025; reporting may lag toxicology / 2026-09-15 | Open interactive; no account needed for public views; data requests by email | Use as the strongest local aggregate mortality source; do not treat the public visualization as a case-level file |
| HCIFS Medical Examiner Case Status, Harris County Institute of Forensic Sciences | [Case Status](https://ifs.harriscountytx.gov/Learning-Center/Case-Status) | Individual case lookup by case number or search fields; no bulk geography | Prior 24 months only / 2026-09-15 | Open lookup; no account found | Report as a documented access limitation; exclude from bulk analysis |
| HCIFS completed autopsy reports, Harris County Institute of Forensic Sciences | [Autopsy report requests](https://ifs.harriscountytx.gov/family-services/Autopsy-Reports) | Individual report, not a published aggregate geography | Record date depends on requested case / 2026-09-15 | Request by email or mail; identifying case details required | Exclude from routine analysis; pursue only an aggregate, de-identified request |
| HCIFS case-level/data records, Harris County Institute of Forensic Sciences | [Media Relations and PIA instructions](https://ifs.harriscountytx.gov/newsroom/Media-Relations) | Not published; possible release scope unknown pending response | Unknown / 2026-09-15 | Written Texas Public Information Act request by email | Report as a gap until the agency confirms whether a de-identified extract exists |
| SAMHSA treatment facilities, FindTreatment.gov | [FindTreatment.gov locator](https://findtreatment.gov/) | Facility-level listings searchable by address; aggregate to ZIP/county for this project | Current listing date not stated / 2026-09-15 | Open public locator; no account needed for search | Use as a supply inventory after deduplication and privacy-preserving geographic aggregation |
| Houston METRO transit data | [METRO developer portal](https://api-portal.ridemetro.org/) | Stop/route/service objects when exposed by the API; no static GTFS file confirmed on the checked public site | Current API vintage not stated / 2026-09-15 | Developer portal/key status requires confirmation | Report static GTFS as unconfirmed; use only after obtaining and pinning a documented feed |
| Naloxone access points, Harris County Public Health | [HCPH Substance Use Data Hub](https://od2a-substance-use-surveillance-hcpublichealth.hub.arcgis.com/) and its public naloxone distribution map | Public map/search product; exact site resolution may be available in the interface but will be aggregated before publication | Vintage not stated / 2026-09-15 | Open interactive; no account needed for public view | Use only if the underlying access-point list and update date can be documented; otherwise report the registry as incomplete |
| Houston open data portal | [City of Houston Open Data](https://data.houstontx.gov/) | Dataset-specific; portal catalog may include point and administrative layers | Dataset-specific / 2026-09-15 | Open catalog | Investigated as a discovery source; use only datasets with documented vintage, geography, and privacy suitability |
| Harris County geospatial open data portal | [Harris County Open Data](https://geo-harriscounty.opendata.arcgis.com/) | Dataset-specific; portal catalog may include county GIS layers | Dataset-specific / 2026-09-15 | Open catalog; public landing page needs no account | Investigated as a discovery source; do not infer that a missing overdose layer exists merely because the portal exists |

The table deliberately includes sources that were not usable. In particular, no public case-level HCIFS file, no confirmed static METRO GTFS feed, and no fully documented public naloxone registry extract were established by this audit.

## 6.3 Analysis plan

### 1. Data environment

Houston/Harris County is **Environment B**, with an aggregate-data / request-based hybrid. HCPH publishes aggregate fatal-overdose trends sourced from HCIFS, Texas DSHS publishes county-level death-certificate measures, CDC provides county-level mortality queries, and HCIFS offers only a limited 24-month case-status lookup plus individual report and PIA request routes. No public bulk case-level overdose or toxicology file was found. The project will not depend on case-level records unless a future request produces a de-identified extract with documented permissions.

### 2. Primary measured quantity

The primary measured quantity will be the annual count and rate of substance-involved deaths published by HCPH for supported Harris County geographies, cross-checked against Texas DSHS death-certificate data. This is an observed administrative mortality quantity, not an inferred need score. The manuscript will distinguish HCPH's HCIFS-based definition from DSHS/NCHS death-certificate definitions and include suppression and reporting-lag caveats.

### 3. Three research questions

- **Where is the burden?** Map and compare HCPH substance-involved death counts/rates at the finest public geography HCPH actually supports, with county-level DSHS/CDC estimates as validation.
- **Where is the service gap?** Combine burden with documented treatment-facility supply, naloxone access points if a dated list can be obtained, transit access if a reproducible METRO feed is obtained, poverty/uninsurance estimates, and SVI. Aggregate facility and access-point records before analysis or publication.
- **Where should supply go?** Rank only supported aggregate units using a transparent composite. Treat the result as planning prioritization, not a causal estimate or proof that a location will reduce deaths.

### 4. Geographic unit

The default analytic unit will be the Harris County ZIP-code geography used by the public HCPH mortality map, because it is the finest geography currently demonstrated for the local mortality product. Census tracts, blocks, and facilities will not be substituted for ZIP-code mortality values. Tract-only layers such as SVI will either remain contextual or be aggregated through a documented, population-weighted crosswalk and labeled modeled. If HCPH cannot export reproducible ZIP-level values, the analysis will fall back to county-level results rather than manufacture tract-level precision.

### 5. Composite and sensitivity variants

The initial composite will use burden 40%, service gap 35%, and vulnerability/barriers 25%. Within each domain, component weights will be equal unless the data inventory justifies another choice. Higher burden, lower supply, longer transit access, higher poverty/uninsurance, and higher SVI will indicate greater priority. Two pre-specified variants will be reported: burden 50% / gap 30% / vulnerability 20%, and burden 30% / gap 45% / vulnerability 25%. Results will report rank correlation, top-area overlap, and rank changes.

### 6. What cannot be computed

This study cannot currently compute individual-level overdose histories, case-level toxicology profiles, exact death locations, causal effects of supply placement, real-time mortality, or a historical HCIFS case panel. It also cannot claim complete naloxone coverage or transit accessibility until the underlying registry/feed and update dates are documented. These limitations will appear in the methods, results, figures, and discussion as findings and uncertainty, not be silently omitted.

## Access classification

| Source | Public without account | Case-level records | Aggregate data | Email/contact | Formal request | Main limitation |
|---|---:|---:|---:|---:|---:|---|
| HCIFS Case Status | Yes | Limited basic lookup | No bulk file found | No | No | Only prior 24 months; not an analytic extract |
| HCIFS autopsy reports | No bulk file found | Individual reports may be requested | No | Yes | Individual request | Identifying case details required; no batch dataset |
| HCIFS public information | No | Unknown pending response | Unknown pending response | Yes | Yes, Texas PIA | Release is not guaranteed and may be restricted |
| HCPH Substance Use Data Hub | Yes | No public case-level table found | Yes | Yes | Optional data request | Interactive/aggregate outputs; source free-text limitations |
| Texas DSHS Health Data | Yes | No | Yes, county/state | Yes | Not needed for dashboard | Death-certificate data, suppression, no toxicology-level rows |
| CDC mortality products | Generally yes | No | Yes | Product-specific | Not needed for standard aggregate use | Death-certificate definitions and suppression |

## What this supports

The project should begin in Environment B unless a successful HCIFS/HCPH data request produces a de-identified case-level or appropriately aggregated extract.

Supported analyses include:

- county-level and other legally/publicly supported aggregate overdose mortality trends;
- aggregate substance-involved death trends by time, demographic group, drug category, and available geography;
- comparison of burden and service access using HCPH, Texas DSHS, CDC, and other public aggregate sources;
- transparent placement prioritization using aggregate burden and access indicators.

Not currently supported by public sources alone:

- individual-level overdose case histories;
- exact overdose locations or addresses;
- case-level toxicology profiles;
- precise point mapping of overdose deaths;
- a reproducible historical HCIFS case-level panel.

## Recommended next request

Before seeking any sensitive records, send a narrowly framed written request to HCIFS and HCPH asking whether they can provide a de-identified, aggregate extract for research. Request geography no finer than the level they can safely support, annual or quarterly time periods, substance categories as already defined by the agency, death circumstances, and suppression rules. Do not request names, addresses, case numbers, exact coordinates, or individual-level records.

The request should ask:

1. whether a de-identified aggregate extract exists;
2. the smallest geography permitted;
3. the time range and update lag;
4. definitions and coding rules for substance involvement;
5. how pending toxicology and late reporting affect counts;
6. suppression and privacy thresholds;
7. whether a data-use agreement, institutional review, registration, fee, or other approval is required.

Until that response is received, cite the public absence precisely: HCIFS publishes a limited case-status lookup and accepts report/PIA requests, but does not expose a public bulk case-level overdose or toxicology dataset.
