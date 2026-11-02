# Municipal Waste Management and Landfill Engineering Project

**Project type:** University engineering study / technical portfolio  
**Main topics:** municipal waste generation, waste composition, material-flow analysis, aerobic stabilization, landfill forecasting, landfill capacity, and wind-rose / green-belt analysis  
**Source material:** four original Excel workbooks and two DWG drawings supplied with the project archive

---

## 1. Executive Summary

This project brings together calculations and technical drawings related to a municipal waste-management system. The supplied materials cover the quantity and composition of generated municipal waste, the distribution of waste streams, the amount of mixed waste considered for aerobic stabilization, the preliminary sizing of stabilization reactors, a 15-year landfill forecast, landfill-area calculations, and a wind-rose / green-belt worksheet.

The baseline waste-generation table reports a population value of **79,000**, an annual waste volume of **122,100 m³/a**, and an annual waste mass of **23,232.2 Mg/a**. The corresponding bulk-density value is approximately **190.27 kg/m³**.

The municipal waste-composition table assigns the largest share to the **organic fraction (44.3%)**, followed by paper (20.2%), fine and mineral fractions (14.0%), glass (10.2%), plastics (6.7%), and metals (4.6%).

The aerobic-stabilization calculation identifies **7,394.67 Mg/a** as the mixed-waste quantity to be stabilized. At the worksheet's assumed density of **650 kg/m³**, this corresponds to approximately **11,376.42 m³/a**, or **218.78 m³/week**. With an assumed stabilization period of eight weeks, the calculated working inventory is approximately **1,750.22 m³**. The source worksheet rounds this to about 1,800 m³ and indicates a requirement of approximately **eight reactors**, based on a nominal single-reactor volume of 234 m³.

The landfill forecast worksheet contains a baseline year of 2026 and a forecast horizon through 2041. It reports an increase in the combined annual volume of household waste and street-cleaning waste from approximately **123.36 thousand m³/a in 2026** to **136.93 thousand m³/a in 2041**.

Several source-sheet inconsistencies remain unresolved, particularly in subgroup labels, waste-composition formulas, the wind-rose observations, and the landfill-area calculation. These are documented in Section 10 and should be settled before any values are treated as final design inputs.

> **Scope statement:** This report documents and organizes the supplied university-project material. It is not a permit application, construction design, operating plan, or independently certified engineering design.

---

## 2. Project Objectives and Scope

The project examines the main stages of a municipal waste-management concept:

1. Estimate the annual amount of municipal waste generated in the study area.
2. Describe the waste composition by material fraction.
3. Organize the waste streams into a mass-flow representation (Sankey diagram).
4. Estimate the amount and volume of mixed waste directed to aerobic stabilization.
5. Estimate the reactor volume and number of reactors required under the stated operating assumptions.
6. Forecast waste quantities over the landfill-planning period.
7. Examine preliminary landfill-volume and site-area assumptions.
8. Review wind-direction data and the proposed green-belt widths.
9. Present the associated technical drawings as supporting engineering documentation.

The supplied files do not provide a fully reconciled design basis for every stage. Therefore, the report distinguishes values transcribed from the source worksheets from arithmetic checks and from items that still require clarification.

---

## 3. Source Material

The original archive contains the following principal files:

| Source file | Content identified in the workbook / file | Role in this report |
|---|---|---|
| `tab.1.xlsx` | Waste generation by area/subgroup, population values, unit generation, annual volume, annual mass, and bulk density | Baseline waste-generation data |
| `tab. 2.xlsx` | Waste composition percentages and calculated mass by fraction | Composition analysis |
| `wykres_Sankeya.xlsx` | Sankey-related workbook and a worksheet titled `obliczenia do Sankeya` | Waste-flow and aerobic-stabilization calculations |
| `Tab 3 Ilość odpadow na składowisko Proj Inst GO - pusty + róża wiatrów + powierzchnia.xlsx` | Landfill forecast, annual volumes, area assumptions, wind-rose data, and green-belt notes | Forecast and environmental/site analysis |
| `Bartosz Sanecki Reaktor rysunek.dwg` | Reactor CAD drawing | Supporting technical drawing |
| `niecka.dwg` | Landfill-basin CAD drawing | Supporting technical drawing |

The source archive also contains embedded previews and images associated with the spreadsheets and drawings. They are supporting illustrations; where a value is unclear in an image, the workbook cell content has been preferred.

---

## 4. Municipal Waste Generation

### 4.1 Baseline data

The baseline table in `tab.1.xlsx` contains the following city-level values:

| Parameter | Source value | Source unit |
|---|---:|---|
| Population / quantity `M` | 79,000 | `M` (unit not expanded in the worksheet) |
| Unit waste volume `Vj` | 1.54557 | m³/Ma |
| Unit waste mass `Qj` | 294.08 | kg/Ma |
| Total annual waste volume | 122,100 | m³/a |
| Total annual waste mass | 23,232.2 | Mg/a |
| Bulk density `ρ` | 190.27 | kg/m³ |

The source notation `m³/Ma` and `kg/Ma` is retained here because the workbook does not expand the abbreviation. It appears to represent a per-inhabitant annual indicator, but that interpretation should be confirmed in the final project documentation.

### 4.2 Area / subgroup breakdown

The first table reports four subgroups:

| Subgroup label in `tab.1.xlsx` | `M` | `Vj` (m³/Ma) | `Qj` (kg/Ma) | Annual volume (m³/a) | Annual mass (Mg/a) | Density (kg/m³) |
|---|---:|---:|---:|---:|---:|---:|
| ZWS | 23,000 | 2.20 | 391.60 | 50,600 | 9,006.8 | 178 |
| ZWN | 43,000 | 1.10 | 209.00 | 47,300 | 8,987.0 | 190 |
| ZC | 8,000 | 2.45 | 514.50 | 19,600 | 4,116.0 | 210 |
| ZJ | 5,000 | 0.92* | 224.48 | 4,600 | 1,122.4 | 244 |

`*` The value `0,92` is stored as text in the source workbook rather than as a numeric cell value. This causes formula errors in the aggregate row shown in the original spreadsheet preview. The value is transcribed as written and should be converted to a numeric value in a corrected calculation file only after the source owner confirms it.

The subgroup populations sum to 79,000, and the subgroup annual masses sum to 23,232.2 Mg/a. The subgroup labels ZC and ZJ are not consistent between the two source tables; see Section 10.

---

## 5. Waste Composition

### 5.1 City-level composition

The city-level row of `tab. 2.xlsx` reports the following composition:

| Waste fraction | Share (%) | Reported mass (Mg/a) |
|---|---:|---:|
| Plastics | 6.7 | 1,556.54 |
| Glass | 10.2 | 2,369.66 |
| Metal | 4.6 | 1,068.67 |
| Paper | 20.2 | 4,692.86 |
| Organic fraction | 44.3 | 10,291.78 |
| Fine and mineral fraction | 14.0 | 3,252.48 |
| **Total** | **100.0** | **approximately 23,232.2** |

The percentages add to 100%. The displayed mass values are rounded; their sum is approximately 23,232.0 Mg/a, which is consistent with the baseline total within rounding differences.

### 5.2 Subgroup composition

The source table also records composition percentages for ZWN, ZWS, ZJ, and ZC. The percentage distributions each add to 100%:

| Subgroup label in `tab. 2.xlsx` | Plastics | Glass | Metal | Paper | Organic | Fine / mineral |
|---|---:|---:|---:|---:|---:|---:|
| ZWN | 5.9% | 10.8% | 3.1% | 24.1% | 36.0% | 20.1% |
| ZWS | 7.6% | 10.1% | 6.0% | 16.0% | 51.0% | 9.3% |
| ZJ | 10.1% | 11.1% | 5.2% | 17.2% | 32.0% | 24.4% |
| ZC | 5.7% | 9.1% | 4.5% | 21.5% | 51.0% | 8.2% |

The subgroup names and some of the mass calculations need to be reconciled before these data are used in a final mass balance. In particular, the ZWN mass row does not correspond to its own percentage distribution and reported total mass. The percentages are therefore presented separately from the unverified subgroup mass outputs.

---

## 6. Waste-Flow Analysis and Sankey Calculations

The `wykres_Sankeya.xlsx` workbook contains a worksheet named `Rys 1 Sankey` and a calculation worksheet named `obliczenia do Sankeya`. The visible numerical material in the calculation worksheet includes the following values:

| Item | Source value | Unit / note |
|---|---:|---|
| Mixed waste stream noted for stabilization, fraction below 80 mm | 11,565.1 | Mg/a; worksheet labels this stream as 100% |
| Associated 40% quantity | 4,626.04 | Mg/a |
| Organic fraction in mixed waste to stabilization | 1,584.95 | Mg/a |
| Mineral fraction | 3,252.51 | Mg/a |
| Other / not separately sorted fraction | 2,557.21 | Mg/a |
| **Sum stated as mixed waste to aerobic stabilization** | **7,394.67** | **Mg/a** |

The three listed components reconcile arithmetically:

\[
1,584.95 + 3,252.51 + 2,557.21 = 7,394.67\;\text{Mg/a}
\]

The original workbook also includes 11,565.1 Mg/a and 4,626.04 Mg/a in the same calculation area. The exact process boundary and relationship between these two values and the 7,394.67 Mg/a stabilization total are not fully explained in the source. They should not be combined or interpreted as separate process outputs without clarifying the Sankey stream definitions.

---

## 7. Aerobic Stabilization Reactor Sizing

### 7.1 Annual and weekly volume

The calculation worksheet uses a bulk density of **650 kg/m³** for the mixed waste directed to aerobic stabilization.

Using the reported mass of 7,394.67 Mg/a:

\[
V_{annual} = \frac{7,394.67\;\text{Mg/a} \times 1,000\;\text{kg/Mg}}{650\;\text{kg/m}^3}
\]

\[
V_{annual} \approx 11,376.42\;\text{m}^3/\text{a}
\]

Assuming 52 weeks per year:

\[
V_{weekly} = \frac{11,376.42}{52} \approx 218.78\;\text{m}^3/\text{week}
\]

### 7.2 Working inventory and reactor count

The source worksheet assumes an aerobic stabilization period of **8 weeks** (and notes a range of 6-12 weeks).

\[
V_{working} = 218.78 \times 8 \approx 1,750.22\;\text{m}^3
\]

The source worksheet rounds this to approximately **1,800 m³**.

The selected single-reactor dimensions appear in the source as **6 m × 3 m × 13 m**, giving:

\[
V_{reactor} = 6 \times 3 \times 13 = 234\;\text{m}^3
\]

Based on the unrounded working inventory:

\[
N = \frac{1,750.22}{234} \approx 7.48
\]

Rounding up to a whole number gives **8 reactors**. The source worksheet also displays 7.6923, which corresponds to the rounded 1,800 m³ divided by 234 m³. Both approaches lead to an eight-reactor preliminary result.

The worksheet additionally contains another dimension combination, **6 m × 4 m × 13 m = 312 m³**, without a clearly stated explanation of whether this is an alternative, an earlier option, or a different internal volume. This needs confirmation.

---

## 8. Landfill Waste Forecast

### 8.1 Forecast basis

The landfill workbook identifies 2026 as the baseline year and notes a 15-year period beginning in 2027 and ending in 2041. It contains working assumptions written in the sheet, including:

- an increase in the city population of +3.2‰;
- a decrease in the municipality population of -2‰;
- a note referring to a +1.5% annual change in city area;
- an increase in the unit waste-volume indicator `Vj` by 0.3 over the 15-year period.

The exact application of every assumption is not fully documented, so the values below are presented as the outputs shown in the source worksheet.

### 8.2 Selected forecast values

| Year | City population (`tys. M`) | City `Vj` (m³/Ma) | City waste volume (`tys. m³/a`) | Street-cleaning waste volume (`tys. m³/a`) | Combined volume shown (`tys. m³/a`) |
|---|---:|---:|---:|---:|---:|
| 2026 | 79.000 | 1.550 | 122.45 | 0.9067 | 123.3567 |
| 2031 | 79.237 | 1.602 | 126.9117 | 0.9819 | 127.8936 |
| 2036 | 79.475 | 1.653 | 131.3991 | 0.9819 | 132.3810 |
| 2041 | 79.714 | 1.705 | 135.9124 | 1.0218 | 136.9341 |

The street-cleaning row uses `Qj = 2 Mg/km²·month` and a density value of `900 kg/m³`. The associated city-area values shown in the source are 34 km² in 2026, 35.3819 km² in 2031, 36.8200 km² in 2036, and 38.3166 km² in 2041.

The source table contains mass outputs (`Qa`, in thousand Mg/a) for selected rows, but some city-year mass cells are blank and the 2031/2036 street-cleaning results appear duplicated despite different area values. These points require checking before the forecast is used as a final landfill design basis.

### 8.3 Annual series and cumulative volume

A separate yearly series runs from 2026 to 2041. It begins at approximately 123.3608 and increases by about 0.9044 per year, reaching approximately 136.0224 in 2040 and 136.9341 in 2041. The sheet also shows a `suma V` value of **1,822.0132** with an adjacent volume label, but the accumulation formula, exact time-period interpretation, and unit basis are not sufficiently clear in the source to treat this as a verified cumulative landfill volume.

---

## 9. Landfill Capacity, Site Area, and Wind-Rose Analysis

### 9.1 Landfill capacity and area

The landfill worksheet includes working parameters and notes such as:

- landfill height `H` options of approximately 8 m, 10 m, and 12 m;
- `Kc` values of 1.5 and 2;
- `Kz` values of 3.5 (compactor), 2.5 (bulldozer), and 1.5 (gravity);
- a note showing an example area of 18.5 ha;
- a calculated area value of **8.3957 ha** labelled as the area of the whole installation.

The wind-rose worksheet separately contains `P = 15.4 ha`. These area values are not reconciled, and the calculation path leading to 8.3957 ha is not sufficiently documented in the supplied sheet. Consequently, this report does not designate one of these values as the final approved landfill area.

### 9.2 Wind-direction data

The wind-rose worksheet records the following directional percentages:

| Direction | N | NE | E | SE | S | SW | W | NW | Calm |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Source frequency (%) | 4 | 12 | 12 | 5 | 5 | 26 | 28 | 5 | 3 |

The directional percentages sum to 97%, with 3% calm conditions, giving 100% in total. The worksheet also calculates corresponding days from a 365-day year. A separate row of observed day counts is provided:

| Direction | N | NE | E | SE | S | SW | W | NW | Calm | Total |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Observed days | 15 | 11 | 25 | 44 | 47 | 84 | 77 | 25 | 37 | 365 |

The two data rows do not represent the same frequency distribution. They should be reconciled by confirming which row is the authoritative observation set and recalculating the percentages from that set.

### 9.3 Green-belt widths

The source worksheet lists the following directional green-belt widths:

| Direction | S | SW | W | NW | N | NE | E | SE |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Width shown (m) | 10 | 25 | 25 | 10 | 20 | 50 | 30 | 10 |

The same worksheet contains notes suggesting 35-50 m for sites above 10 ha, 25-35 m for sites below 10 ha, and a note of 10 m as a minimum. No legal or regulatory source is supplied next to these notes. They are therefore recorded as project assumptions / notes, not as confirmed regulatory requirements.

---

## 10. Data-Quality Review and Items Requiring Confirmation

The following issues are visible in the supplied files. They are not silently corrected in this report.

| ID | Source location | Issue observed | Required follow-up |
|---|---|---|---|
| DQ-01 | `tab.1.xlsx`, city aggregate row | The `ZJ` unit-volume value `0,92` is stored as text. The original preview shows `#VALUE!` errors in calculated cells. | Confirm the intended numeric value and convert it to a numeric cell before recalculating the aggregate row. |
| DQ-02 | `tab.1.xlsx` vs `tab. 2.xlsx` | Subgroup labels `ZC` and `ZJ` are associated with different mass totals across the two workbooks. In `tab.1.xlsx`, ZC = 4,116 Mg/a and ZJ = 1,122.4 Mg/a; in `tab. 2.xlsx`, the composition rows label 4,116 as ZJ and 1,122.4 as ZC. | Confirm the correct ZC/ZJ assignment and update all linked tables consistently. |
| DQ-03 | `tab. 2.xlsx`, ZWN row | The percentages total 100%, but the reported mass values for the organic and fine/mineral fractions do not match the stated percentages and the ZWN total of 8,987 Mg/a. | Recalculate subgroup mass by applying each percentage to the correct subgroup mass after confirming the label. |
| DQ-04 | `wykres_Sankeya.xlsx`, `obliczenia do Sankeya` | The connection between 11,565.1 Mg/a, 4,626.04 Mg/a (40%), and the 7,394.67 Mg/a stabilization total is not fully defined. | Clarify the stream boundaries and process stages represented by each value; check that Sankey flows balance. |
| DQ-05 | `wykres_Sankeya.xlsx`, reactor sizing | Both 6 × 4 × 13 m = 312 m³ and 6 × 3 × 13 m = 234 m³ are shown. The displayed 7.6923 reactor count is based on rounded 1,800 m³ / 234 m³, while the unrounded 1,750.22 m³ / 234 m³ gives about 7.48. | Confirm which reactor dimensions are intended and retain the round-up to eight only if the 234 m³ volume is selected. |
| DQ-06 | Landfill forecast worksheet | Some annual mass cells are blank. The 2031 and 2036 street-cleaning values appear duplicated although the area values differ. | Check formulas and complete the missing year calculations. |
| DQ-07 | Landfill capacity / wind-rose worksheets | The source includes 8.3957 ha, 15.4 ha, and an example of 18.5 ha without a reconciled basis. | Rebuild the site-area calculation with explicit assumptions, geometry, compaction factors, and time horizon. |
| DQ-08 | Wind-rose worksheet | The percentage row and observed day-count row do not match. The observed counts sum to 365 days, but their directional proportions differ from the percentage row. | Select the authoritative dataset and recalculate frequencies and wind-rose values consistently. |
| DQ-09 | Wind-rose worksheet | Green-belt width notes refer to thresholds and minimum values but contain no cited regulation or technical source. | Add the applicable regulatory / planning reference or label the widths as assumptions only. |
| DQ-10 | Landfill forecast worksheet | The `suma V = 1,822.0132` value is not clearly tied to a documented annual-series summation and unit basis. | Verify the formula, period included, and units before using it as the required landfill volume. |

---

## 11. Conclusions

The supplied material provides a useful foundation for a municipal waste-management engineering study. It connects waste-generation estimates and waste composition with a proposed treatment route, preliminary aerobic-stabilization sizing, and landfill-planning calculations. The two DWG files provide supporting technical drawings for the reactor and landfill basin.

The baseline data indicate a city-level municipal waste quantity of approximately **23,232.2 Mg/a**. The composition table identifies the organic fraction as the largest single category at **44.3%**. The stabilization worksheet gives a preliminary annual stabilization quantity of **7,394.67 Mg/a**, corresponding to a calculated working inventory of about **1,750 m³** for an eight-week stabilization period. With the 234 m³ reactor volume shown in the source, the preliminary requirement rounds up to **eight reactors**.

The landfill worksheet suggests that combined annual waste volume increases from approximately **123.36 thousand m³/a** in 2026 to **136.93 thousand m³/a** in 2041. However, the final cumulative volume and site area are not sufficiently reconciled to be stated as verified results. The wind-rose worksheet also requires reconciliation between the percentage distribution and observed day counts.

The most important next step is to resolve the data-quality items in Section 10. In particular, the subgroup labels, ZWN composition masses, stabilization flow boundaries, cumulative landfill volume, landfill area, and wind-rose dataset should be confirmed. Once those matters are resolved, the calculations and drawings can be presented as one coherent engineering portfolio case study.

---

## 12. Disclaimer

This document is a structured summary of the original university-project materials and a limited arithmetic review of selected values. It does not certify the completeness or correctness of the underlying engineering design. Waste-treatment capacity, reactor operation, landfill geometry, environmental protection distances, wind-rose interpretation, and regulatory compliance require project-specific verification and appropriate source documentation.

**Prepared for:** Engineering portfolio presentation  
**Project status:** Source material organized and reviewed; selected calculation and data inconsistencies remain open for confirmation.
