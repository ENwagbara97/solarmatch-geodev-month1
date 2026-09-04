# SolarMatch — Preliminary Geospatial Screening for Decentralized Energy Opportunities

## GeoDev Lab Africa — Month 1 Project

### Project Status

Month 1 — Project Definition and Data Preparation

---

## 1. Project Overview

SolarMatch is a long-term geospatial decision-support concept focused on helping identify and understand potential opportunities for decentralized renewable energy deployment in Nigeria.

For Month 1 of GeoDev Lab Africa, the project is deliberately limited to a preliminary spatial screening study.

The goal is not to determine where a solar mini-grid should ultimately be built.

Instead, this study asks whether available Nigerian geospatial data can be used to identify settlements that show preliminary spatial characteristics worth further investigation for decentralized solar energy development.

---

## 2. Spatial Question

> Which settlements in Nsit Ibom Local Government Area, Akwa Ibom State, show preliminary potential for decentralized solar energy development based on solar resource, population distribution, settlement location, and proximity to road infrastructure?

---

## 3. Study Area

### Nsit Ibom Local Government Area

State: Akwa Ibom State  
Country: Nigeria

Nsit Ibom was selected as a manageable study area for the Month 1 investigation. Limiting the analysis to one Local Government Area keeps the project small enough to complete while providing a realistic Nigerian setting for testing the SolarMatch concept.

The study area may be expanded in later stages after the Month 1 workflow has been validated.

---

## 4. Why This Question Matters

Identifying locations for decentralized energy projects requires more than knowing where solar resources are available.

Potential locations also need to be considered in relation to:

- where people live
- population concentration
- settlement distribution
- accessibility
- existing infrastructure
- terrain
- electricity access
- environmental and land constraints
- technical feasibility
- economic viability

This Month 1 project focuses only on a small subset of these factors.

The purpose is to establish a reliable geospatial foundation that can later be expanded into a broader SolarMatch decision-support workflow.

---

## 5. Month 1 Scope

### Included

- Study area boundary
- Settlement locations
- Population distribution
- Solar resource
- Road infrastructure
- Basic spatial relationships
- Coordinate reference system checks
- Preliminary spatial screening

### Not included yet

- Detailed solar PV system design
- Electrical engineering design
- Detailed load modelling
- Distribution network design
- Land ownership or land availability assessment
- Environmental and social impact assessment
- Community consent
- Financial feasibility
- Final investment decisions
- Regulatory approval

The Month 1 output should therefore be interpreted as a preliminary geospatial screening result, not a final site recommendation.

---

## 6. Datasets

| Dataset | Purpose | Source |
|---|---|---|
| Nigeria Administrative Boundaries | Define and extract the Nsit Ibom study area | ENERGYDATA.INFO / Humanitarian Data Exchange |
| Solar Resource Data | Represent available solar resource | Global Solar Atlas |
| Population Raster | Represent population distribution and potential energy demand | WorldPop |
| Settlement Data | Identify populated places and settlement locations | OpenStreetMap |
| Road Network | Represent accessibility to existing road infrastructure | OpenStreetMap |

### Dataset Sources

**Nigeria Administrative Boundaries**

https://energydata.info/en/dataset/nigeria-administrative-boundaries-2017

**Global Solar Atlas**

https://dev.globalsolaratlas.info/support/data-sources

**WorldPop — Nigeria Population Counts**

https://hub.worldpop.org/geodata/summary?id=74736

**OpenStreetMap — Export**

https://www.openstreetmap.org/export/

**OpenStreetMap — Downloading Data**

https://wiki.openstreetmap.org/wiki/Downloading_data

---

## 7. Planned Spatial Workflow

The Month 1 workflow will follow:

Question
→ Data discovery
→ Data download
→ Data inspection
→ Data cleaning
→ CRS verification
→ Study area extraction
→ Spatial analysis
→ Preliminary result
→ Documentation

The first analysis will focus on spatial relationships between settlements and road infrastructure while incorporating available population and solar-resource information.

The exact analytical operation will be confirmed after inspecting the downloaded datasets rather than assuming that every dataset can be used in the same way.

---

## 8. Expected Output

The Month 1 project is expected to produce:

1. A cleaned study-area boundary
2. Mapped settlement locations
3. Population distribution
4. Solar-resource information
5. Road infrastructure
6. A preliminary spatial screening result
7. A documented GIS workflow
8. A reproducible project repository

---

## 9. Expected Map

The main map should communicate:

- Nsit Ibom study area
- settlements
- population distribution
- road network
- solar-resource variation
- preliminary areas identified for further investigation

The final map will not represent a construction recommendation.

---

## 10. Important Assumptions

This project assumes that:

- available datasets provide sufficient spatial coverage for the study area
- settlement locations are sufficiently represented in the selected source
- population estimates can be used as an indicative representation of potential demand
- solar-resource data can provide a useful first-level indication of solar potential
- road proximity can serve as one preliminary accessibility indicator

These assumptions will be reviewed as the project develops.

---

## 11. Limitations

The result will be affected by:

- differences in dataset dates
- differences in spatial resolution
- incomplete or outdated OpenStreetMap features
- uncertainty in population estimates
- limitations of publicly available electricity infrastructure data
- absence of detailed land ownership information
- absence of detailed community-level electricity demand data
- lack of site-specific engineering surveys

Therefore, a high preliminary score should not be interpreted as proof that a site is technically, financially, socially, or legally suitable for development.

---

## 12. Long-Term SolarMatch Direction

The Month 1 study is the first stage of a larger SolarMatch concept.

Future stages may incorporate:

- electricity access
- existing grid infrastructure
- distribution network proximity
- solar PV potential
- population and demand
- productive-use facilities
- road accessibility
- terrain
- flood and environmental constraints
- land-use information
- community considerations
- estimated project capacity
- project economics
- investment screening

The long-term goal is to develop a geospatial decision-support workflow that helps users move from:

**Where is the opportunity?**

to:

**Why is it an opportunity?**

and eventually:

**What should be investigated next?**

---

## 13. Relationship to Existing Electrification Planning

SolarMatch does not assume that existing electrification planning tools or government programmes do not exist.

Nigeria already has geospatial electrification resources, including the World Bank's Global Electrification Platform and Distributed Renewable Energy Atlas.

These resources demonstrate the value of combining spatial data with energy planning.

SolarMatch will therefore be developed as a complementary screening and decision-support concept rather than as a replacement for official planning, engineering studies, regulatory processes, or investment due diligence.

---

## 14. Reproducibility

All datasets, sources, processing decisions, assumptions, and analytical steps will be documented as the project develops.

Where dataset licenses permit redistribution, processed data or references to the original source will be documented in the repository.

Large or externally hosted datasets will not necessarily be committed directly to GitHub.

---

## 15. Month 1 Learning Objectives

Through this project I aim to learn and demonstrate:

- how to define a spatial question
- how to identify obtainable Nigerian datasets
- how to inspect vector and raster data
- how to work with attributes
- how to correctly handle coordinate reference systems
- how to perform basic spatial analysis
- how to document a GIS workflow
- how to produce a reproducible geospatial project

---

## 16. Project Owner

**Nwagbara Ebubechukwu**

GeoDev Lab Africa — Cohort One