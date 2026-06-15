# Wind Farm Site Selection — Denmark

An interactive multi-criteria evaluation (MCE) of wind farm suitability across Denmark, with sensitivity analysis using a coefficient of variation (CV) heatmap across 66 weight combinations.

## Interactive Map

**[View the map](https://satheendra.github.io/MCE_WindFarm_DK/)**

## Study Area

Denmark, analysed at 50 m spatial resolution in UTM Zone 32N (EPSG:32632). After applying a land cover exclusion mask derived from CORINE Land Cover (2018), the permitted analysis domain covers 3,827 km².

## Suitability Criteria

| Key | Criterion | Weight (S1 baseline) |
|-----|-----------|----------------------|
| P | Distance to powerlines | 0.36 |
| R | Distance from roads | 0.18 |
| S | Terrain slope | 0.46 |

Weights were derived using the Analytic Hierarchy Process (AHP). Each criterion was reclassified onto a 0–100 suitability scale before weighted linear combination (WLC).

## Scenarios

| Scenario | Description | P | R | S |
|----------|-------------|-----|-----|-----|
| S1 | Baseline (AHP) | 0.36 | 0.18 | 0.46 |
| S2 | Optimal distance to powerlines | 0.55 | 0.15 | 0.30 |
| S3 | Optimal distance from roads | 0.30 | 0.45 | 0.25 |
| S4 | Equally weighted criteria | 0.33 | 0.33 | 0.34 |

## Sensitivity Analysis

A CV heatmap was computed across 66 weight combinations (each weight varied from 0.0 to 1.0 in steps of 0.1). Sites with mean suitability ≥ 60 and CV ≤ 30% were retained as final proposals. This produced **140 candidate sites** covering approximately **1,070 km²**.

## Data Sources

- **Roads and powerlines:** OpenStreetMap (ODbL 1.0)
- **Land cover exclusion mask:** CORINE Land Cover, version 2018
- **Elevation / slope:** Digital Terrain Model (~30 m), resampled to 50 m

## Repository Structure
