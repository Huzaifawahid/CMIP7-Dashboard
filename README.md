# CMIP7 Data Visualisation Dashboard

> An interactive Excel workbook for exploring global climate projections across seven CMIP7 ScenarioMIP emission pathways (2000–2100).

---

## Overview

This dashboard provides an interactive interface for visualising key climate indicators derived from the CMIP7 ScenarioMIP scenarios, as described in Van Vuuren et al. (2026). It is designed to support researchers, policymakers, and educators in comparing emission trajectories, radiative forcing, atmospheric concentrations, and projected temperature outcomes across a range of plausible futures — from high-end warming to net-negative pathways.

---

## Citation

> Van Vuuren, D. P., O'Neill, B. C., Tebaldi, C., et al. (2026). *The Scenario Model Intercomparison Project for CMIP7 (ScenarioMIP-CMIP7)*. Geoscientific Model Development, 19, 2627–2656. https://doi.org/10.5194/gmd-19-2627-2026

**Data source:** CMIP7 Scenario Explorer

---

## Scenarios

The dashboard covers all seven CMIP7 ScenarioMIP pathways, spanning projected warming of ~1.5 °C to ~3.5 °C above the 1850–1900 baseline by 2100.

| Label | Full name | Description |
|-------|-----------|-------------|
| **H** | High | Emissions grow as high as plausibly possible; strong warming, no policy action |
| **HL** | High-to-Low | Emissions rise initially then sharply decline, reaching net-zero by 2100 |
| **M** | Medium | Current policies maintained from 2025; moderate warming |
| **ML** | Medium-to-Low | Gradual emissions reduction; net-zero by end of century |
| **L** | Low | Consistent with likely keeping warming below 2 °C |
| **VL** | Very Low | Deep cuts limiting warming to ~1.5 °C with limited overshoot |
| **LN** | Low-to-Negative | Slight overshoot of 1.5 °C, then rapid net-negative emissions to bring warming back down |

---

## Climate Indicators

The dashboard visualises the following indicators across all scenarios:

| Indicator | Unit |
|-----------|------|
| CO₂ annual emissions (FFI + AFOLU) | GtCO₂ yr⁻¹ |
| Cumulative CO₂ emissions | GtCO₂ |
| CH₄ emissions | TgCH₄ yr⁻¹ |
| N₂O emissions | TgN₂O yr⁻¹ |
| GHG emissions (CO₂-equivalent) | GtCO₂eq yr⁻¹ |
| Short-lived climate forcers (Sulfur, BC, OC, NOx, VOC, NH₃, CO) | Native FAIR units yr⁻¹ |
| Halogenated gases (CFCs, HCFCs, HFCs, PFCs, SF₆, NF₃) | Native FAIR units yr⁻¹ |
| Effective radiative forcing | W m⁻² |
| Aerosol–radiation interactions | W m⁻² |
| Atmospheric CO₂ concentration | ppm |
| Global mean temperature anomaly (vs. 1850–1900) | °C |

---

## Workbook Structure

```
CMIP7_Dashboard.xlsm
├── Dashboard               ← Main interactive view with charts and controls
├── Emissions Analysis      ← Pivot tables by gas and scenario
├── Emissions               ← Raw annual emissions data (2000–2100)
├── Projections_table       ← Forcing and concentration projections
├── Climate Projections     ← Radiative forcing outputs
├── Temperature             ← Warming anomaly by scenario
├── helper table            ← Back-end calculations for emissions charts
└── temp helper table       ← Back-end calculations for temperature charts
```

---

## Requirements

- Microsoft Excel (2016 or later) with **macros enabled**
- The file uses `.xlsm` format — macro content must be enabled on first open for interactive controls to function

> **Note:** On first open, Excel may show a security warning. Click **Enable Content** to activate the dashboard controls.

---

## Getting Started

1. Download `CMIP7_Dashboard.xlsm` from this repository
2. Open in Microsoft Excel and click **Enable Content** when prompted
3. Navigate to the **Dashboard** sheet
4. Use the **Scenario Legend** panel to toggle scenarios on/off
5. Use the **Indicators** and **Select Gas** controls to switch between variables

---

## License

This dashboard was developed for research and educational purposes. Data are sourced from the CMIP7 Scenario Explorer under the terms of the CMIP7 data usage policy. Please cite Van Vuuren et al. (2026) when using this dashboard in publications or presentations.

---

## Contact

For questions or feedback, please open an issue in this repository.
