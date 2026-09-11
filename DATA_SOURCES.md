# SolarMatch — Week 2 Data Acquisition Guide

This file records exactly where the Month 1 datasets come from and how they should be acquired before opening them in QGIS.

## 1. Administrative boundaries

**Source:** ENERGYDATA.INFO / HDX — Nigeria Administrative Boundaries 2017  
**Link:** https://energydata.info/en/dataset/nigeria-administrative-boundaries-2017

Use the LGA boundary layer to identify and extract **Nsit Ibom LGA**.

## 2. Settlements

**Source:** OpenStreetMap  
**Link:** https://www.openstreetmap.org/export/

**Recommended QGIS method:** QuickOSM → Key: `place` → Value: relevant populated-place classes such as `village`, `town`, `hamlet` → restrict the query to Nsit Ibom.

## 3. Roads

**Source:** OpenStreetMap  
**Link:** https://www.openstreetmap.org/export/

**Recommended QGIS method:** QuickOSM → Key: `highway` → Value: `*` → restrict the query to Nsit Ibom.

## 4. Population

**Source:** WorldPop — Nigeria population grid  
**Link:** https://hub.worldpop.org/geodata/summary?id=74736

The selected product is a roughly 100 m population grid. Download the GeoTIFF and inspect its raster properties in QGIS before using it.

## 5. Solar resource

**Source:** Global Solar Atlas  
**Data-source information:** https://dev.globalsolaratlas.info/support/data-sources  
**FAQ:** https://www.globalsolaratlas.info/support/faq

For this Month 1 screening, use a solar-resource layer such as GHI. Download the appropriate GIS raster and inspect its properties in QGIS.

## Acquisition rule

Do not invent feature counts, field names, raster dimensions, NoData values or value ranges. These belong in `DATA_NOTE.md` only after the actual downloaded files have been inspected in QGIS.

## GitHub data-size note

Large GeoTIFFs and other binary geospatial files may be unsuitable for ordinary GitHub repository storage. If a source raster is too large, document the original source and acquisition steps instead of forcing the binary into the repository. Processed, clipped files should only be committed when their size and licensing make that practical.
