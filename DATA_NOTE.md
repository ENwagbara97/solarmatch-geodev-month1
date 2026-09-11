# SolarMatch — Week 2 Data Note

## Project

**Project:** SolarMatch — Preliminary Geospatial Screening for Decentralized Energy Opportunities  
**Study area:** Nsit Ibom Local Government Area, Akwa Ibom State, Nigeria  
**Programme:** GeoDev Lab Africa — Month 1

## Purpose of this note

This note records the datasets selected for the Week 2 data work. The project uses vector and raster data, so the inspection fields differ slightly by data type: vector datasets are described by feature count, geometry and attributes, while raster datasets are described by pixel resolution, CRS, bands and value/NoData information.

> **Important:** Feature counts and raster statistics below must be taken from the actual files after they are downloaded and opened in QGIS. They should not be guessed from the source catalogue.

---

## 1. Nigeria Administrative Boundaries

**Purpose:** Define the Nsit Ibom LGA study area and provide the boundary used to extract/clip other datasets.

**Source:** ENERGYDATA.INFO / Humanitarian Data Exchange (HDX)  
**Source link:** https://energydata.info/en/dataset/nigeria-administrative-boundaries-2017  
**Resource:** Local Government Areas (LGA) Boundary  
**Source format:** SHP ZIP, with GeoJSON also provided as an alternate format.  
**License:** Creative Commons Attribution 4.0

**Expected geometry:** Polygon  
**Feature count:** To be recorded from the downloaded layer in QGIS.  
**Key columns:** To be recorded from the downloaded layer in QGIS; the LGA name field will be used to identify Nsit Ibom.  
**Missing/gap observations:** To be checked in QGIS, particularly for missing LGA names or attributes and whether Nsit Ibom is represented correctly.

---

## 2. Settlement Data

**Purpose:** Represent populated places within Nsit Ibom and support the spatial screening of settlements.

**Source:** OpenStreetMap (OSM)  
**Source link:** https://www.openstreetmap.org/export/  
**Download guidance:** https://wiki.openstreetmap.org/wiki/Downloading_data

**Acquisition method:** QGIS QuickOSM, using OpenStreetMap features relevant to populated places (for example `place` categories such as village, town and hamlet).

**Expected geometry:** Point  
**Feature count:** To be recorded from the actual QuickOSM output in QGIS.  
**Key columns:** To be recorded from the actual QuickOSM output; expected useful fields include `name` and `place` where present.  
**Missing/gap observations:** OSM coverage is community-maintained, so missing names, incomplete place classifications or uneven mapping may occur. These will be recorded after inspection rather than assumed.

---

## 3. Road Network

**Purpose:** Represent road infrastructure and provide a preliminary accessibility variable for the spatial screening.

**Source:** OpenStreetMap (OSM)  
**Source link:** https://www.openstreetmap.org/export/  
**Download guidance:** https://wiki.openstreetmap.org/wiki/Downloading_data

**Acquisition method:** QGIS QuickOSM using the `highway` key for the Nsit Ibom study area.

**Expected geometry:** LineString / MultiLineString depending on the QuickOSM output.  
**Feature count:** To be recorded from the actual QuickOSM output in QGIS.  
**Key columns:** To be recorded from the actual QuickOSM output; `highway`, `name` and other available road attributes will be inspected.  
**Missing/gap observations:** OSM road mapping may be incomplete or uneven. Road classifications and unnamed roads will be checked during inspection.

---

## 4. Population Raster

**Purpose:** Represent population distribution as an indicator of the number of people potentially served by decentralized energy interventions.

**Source:** WorldPop — Nigeria Spatial Distribution of Population  
**Source link:** https://hub.worldpop.org/geodata/summary?id=74736  
**Dataset:** Nigeria population estimates for 2026, R2025A version v1.  
**Format:** GeoTIFF  
**Resolution:** 3 arc-seconds, approximately 100 m  
**CRS:** Geographic Coordinate System, WGS84 (EPSG:4326)  
**Units:** Estimated number of people per grid cell

**Raster dimensions:** To be recorded from the downloaded file in QGIS.  
**Bands:** To be recorded from the downloaded file.  
**NoData/value range:** To be recorded from the downloaded file.  
**Missing/gap observations:** To be checked after loading the raster and clipping/inspecting the Nsit Ibom extent.

**Note:** The WorldPop page describes this R2025A product as an alpha version that may change as improvements are made.

---

## 5. Solar Resource

**Purpose:** Represent available solar resource as one preliminary indicator of decentralized solar potential.

**Source:** Global Solar Atlas / Solargis / World Bank  
**Source link:** https://dev.globalsolaratlas.info/support/data-sources  
**Additional guidance:** https://www.globalsolaratlas.info/support/faq

**Selected variable:** Global Horizontal Irradiation (GHI)  
**Format:** GeoTIFF  
**CRS:** EPSG:4326  
**Nominal resolution:** 9 arc-seconds (approximately 250 m) for solar-resource data

**Raster dimensions:** To be recorded from the downloaded file in QGIS.  
**Bands:** To be recorded from the downloaded GHI file.  
**NoData/value range:** To be recorded from the downloaded file.  
**Missing/gap observations:** To be checked after loading and inspecting the Nsit Ibom extent.

**Important:** GHI is a solar-resource indicator, not a complete measure of actual PV project feasibility. The project will not treat GHI alone as a final site recommendation.

---

## Week 2 Inspection Checklist

For each vector layer, record:

- actual feature count
- geometry type
- important attribute/column names
- missing or empty values
- unexpected categories or duplicate-looking records
- whether the study area is adequately covered

For each raster layer, record:

- CRS
- pixel size/resolution
- rows and columns
- number of bands
- NoData value
- minimum and maximum values where useful
- whether the study area is adequately covered

## General observations

The selected datasets have different sources, dates, resolutions and levels of completeness. These differences will be documented during QGIS inspection rather than hidden. OpenStreetMap coverage is particularly subject to changes and local mapping completeness.

## Week 2 status

The repository is prepared for the Week 2 data note. The actual feature counts, attribute names and raster statistics should be filled from the files after the datasets have been downloaded and opened in QGIS.
