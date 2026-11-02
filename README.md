# Engineering Projects

A portfolio of engineering projects, most of which were completed during my university studies. The work covers **building services (HVAC)**, **renewable energy simulation**, and **municipal waste management**. It combines 2D CAD drafting in AutoCAD, simulation in specialized engineering software, spreadsheet-based calculations, and technical reporting.

> **Background:** Most projects were originally completed as coursework during my engineering studies. Some were later extended or reorganized for portfolio presentation.
>
> **Scope:** All projects are educational and portfolio studies. Drawings, calculations, and simulation results are illustrative and are not construction, permitting, or installation documentation.

---

## Projects at a glance

| # | Project | Domain | Main tools | Deliverables |
|---|---|---|---|---|
| 01 | [AutoCAD Residential HVAC Systems](./01_AutoCAD_Residential_HVAC_Systems_Project/) | Building services / heating | AutoCAD | 3 DWG schematics and PNG previews |
| 02 | [Municipal Waste Management and Landfill Engineering](./02_Municipal_Waste_Management_Project/) | Environmental engineering | Excel, AutoCAD | 2 DWG drawings, 3 XLSX workbooks, Sankey diagram, technical report |
| 03 | [GeoT*SOL Heat Pump System Design](./03_GeoTSOL_Heat_Pump_System_Design/) | Heat pumps / energy simulation | GeoT*SOL 2025 R1 | 4 simulation reports (PDF) |
| 04 | [PV*SOL Photovoltaic System Design](./04_PVSOL_Photovoltaic_System_Design/) | Photovoltaics / energy simulation | PV*SOL 2025 | 4 simulation reports (PDF) |

---

## 01 - AutoCAD Residential HVAC Systems

Three 2D schematics compare different ways of supplying space heating and domestic hot water (DHW) to a residential building with underfloor heating:

1. Air-to-water heat pump - split system (Panasonic Aquarea R32).
2. Air-to-water heat pump - monobloc system.
3. Gas condensing boiler system.

**Work performed:** equipment representation and symbols, orthogonal pipe routing, colour-coded heating, DHW and refrigerant lines, manifold connections, labels, leaders, and legends.

**Outcome:** three consistently drafted system schematics that allow the main system concepts to be compared.

### Drawing previews

<table>
  <tr>
    <td width="33%"><img src="./01_AutoCAD_Residential_HVAC_Systems_Project/Previews/01_Panasonic_Aquarea_Split_R32_Underfloor_Heating.png" alt="Panasonic Aquarea split heat pump schematic" width="100%"></td>
    <td width="33%"><img src="./01_AutoCAD_Residential_HVAC_Systems_Project/Previews/02_Air_to_Water_Monobloc_Underfloor_Heating.png" alt="Air-to-water monobloc heat pump schematic" width="100%"></td>
    <td width="33%"><img src="./01_AutoCAD_Residential_HVAC_Systems_Project/Previews/03_Gas_Condensing_Boiler_Underfloor_Heating.png" alt="Gas condensing boiler schematic" width="100%"></td>
  </tr>
  <tr>
    <td align="center">Split heat pump</td>
    <td align="center">Monobloc heat pump</td>
    <td align="center">Gas condensing boiler</td>
  </tr>
</table>

[Open project folder](./01_AutoCAD_Residential_HVAC_Systems_Project/)

---

## 02 - Municipal Waste Management and Landfill Engineering

A municipal waste management study for a town of approximately **79,000 inhabitants**, with an estimated annual waste stream of **23,232 Mg** and an organic fraction of **44.3%**.

The project covers:

- Waste generation and composition analysis.
- A waste-flow **Sankey diagram**, covering selective collection, sorting, stabilization, compost, and landfilled fractions.
- Preliminary sizing of **aerobic stabilization reactors**: approximately **7,394.67 Mg/year** of material to stabilize and an estimated configuration of **8 reactors**, each with a volume of approximately **234 m³**.
- A **15-year landfill forecast** covering 2026-2041, with preliminary capacity and area analysis.
- Wind-rose and green-belt review.
- 2D CAD drawings of the **reactor** and **landfill basin**.

**Outcome:** a workflow from waste data analysis to a treatment concept and preliminary site layout. The technical report documents the methodology and identifies inconsistencies or limitations in the source data, rather than presenting uncertain inputs as verified facts.

### Selected project visuals

<table>
  <tr>
    <td width="50%"><img src="./02_Municipal_Waste_Management_Project/Previews/Sankey.png" alt="Municipal waste flow Sankey diagram" width="100%"></td>
    <td width="50%"><img src="./02_Municipal_Waste_Management_Project/Previews/Landfill_Forecast.png" alt="Landfill basin and forecast drawing" width="100%"></td>
  </tr>
  <tr>
    <td align="center">Waste-flow Sankey diagram</td>
    <td align="center">Landfill forecast drawing</td>
  </tr>
  <tr>
    <td colspan="2"><p align="center"><img src="./02_Municipal_Waste_Management_Project/Previews/Reactor.png.png" alt="Aerobic stabilization reactor CAD drawing" width="55%"></p></td>
  </tr>
  <tr>
    <td colspan="2" align="center">Aerobic stabilization reactor drawing</td>
  </tr>
</table>

[Open project folder](./02_Municipal_Waste_Management_Project/) · [Read technical report](./02_Municipal_Waste_Management_Project/Report.md)

---

## 03 - GeoT*SOL Heat Pump System Design

A comparative simulation study of residential **air-to-water heat pump systems** created in **GeoT*SOL 2025 R1**. Four scenarios compare two household sizes (2+2 and 2+4) in two Polish locations: Olsztyn and Rzeszów.

| Scenario | Heated area | Heat pump SPF | Annual heat pump electricity | CO₂ avoided |
|---|---:|---:|---:|---:|
| 2+2 - Olsztyn | 116 m² | 3.0 | 4,728 kWh | 2,457 kg |
| 2+2 - Rzeszów | 116 m² | 3.2 | 4,166 kWh | 2,322 kg |
| 2+4 - Olsztyn | 130 m² | 2.9 | 6,516 kWh | 4,257 kg |
| 2+4 - Rzeszów | 130 m² | 3.0 | 6,437 kWh | 4,263 kg |

**Work performed:** configuration of heat pumps and hot-water storage, definition of space-heating and DHW demand, annual energy simulation, review of photovoltaic contribution, and comparison of system performance and environmental indicators.

**Result comparison:** the Rzeszów scenarios show slightly higher SPF values than the corresponding Olsztyn scenarios in these simulations. This describes the specific modeled configurations and should not be treated as a general conclusion about the two locations.

### Simulation reports

- [2+2 household - Olsztyn (PDF)](./03_GeoTSOL_Heat_Pump_System_Design/Dom%20(2%2B2)%20-%20Olsztyn%20-%20GeoTSOL.pdf)
- [2+2 household - Rzeszów (PDF)](./03_GeoTSOL_Heat_Pump_System_Design/Dom%20(2%2B2)%20-%20Rzesz%C3%B3w%20-%20GeoTSOL.pdf)
- [2+4 household - Olsztyn (PDF)](./03_GeoTSOL_Heat_Pump_System_Design/Dom%20(2%2B4)%20-%20Olsztyn%20-%20GeoTSOL.pdf)
- [2+4 household - Rzeszów (PDF)](./03_GeoTSOL_Heat_Pump_System_Design/Dom%20(2%2B4)%20-%20Rzesz%C3%B3w%20-%20GeoTSOL.pdf)

[Open project folder](./03_GeoTSOL_Heat_Pump_System_Design/)

---

## 04 - PV*SOL Photovoltaic System Design

A comparative design and simulation study of grid-connected residential photovoltaic systems created in **PV*SOL 2025**. Four scenarios cover the same two household sizes (2+2 and 2+4) and locations (Olsztyn and Rzeszów).

| Scenario | PV capacity | Annual production | Self-consumed energy | Exported energy | CO₂ avoided |
|---|---:|---:|---:|---:|---:|
| 2+2 - Olsztyn | 6.32 kWp | 6,326 kWh | 1,525 kWh | 4,801 kWh | 2,378 kg |
| 2+2 - Rzeszów | 5.14 kWp | 5,472 kWh | 1,420 kWh | 4,052 kWh | 2,062 kg |
| 2+4 - Olsztyn | 9.28 kWp | 9,730 kWh | 1,937 kWh | 7,793 kWh | 4,560 kg |
| 2+4 - Rzeszów | 8.70 kWp | 9,462 kWh | 1,850 kWh | 7,612 kWh | 4,435 kg |

**Work performed:** PV module and inverter selection, definition of module orientation and tilt, roof-area allocation, string configuration, climate-data review using Meteonorm 8.2, annual yield simulation, and financial analysis including investment cost, IRR, and estimated payback period.

**Outcome:** four comparable PV system simulations showing annual production, on-site energy use, grid exports, and selected financial and environmental indicators.

### Simulation reports

- [2+2 household - Olsztyn (PDF)](./04_PVSOL_Photovoltaic_System_Design/PVSOL%20(2%2B2)%20Olsztyn.pdf)
- [2+2 household - Rzeszów (PDF)](./04_PVSOL_Photovoltaic_System_Design/PVSOL%20(2%2B2)%20Rzesz%C3%B3w.pdf)
- [2+4 household - Olsztyn (PDF)](./04_PVSOL_Photovoltaic_System_Design/PVSOL%20(2%2B4)%20Olsztyn.pdf)
- [2+4 household - Rzeszów (PDF)](./04_PVSOL_Photovoltaic_System_Design/PVSOL%20(2%2B4)%20Rzesz%C3%B3w.pdf)

[Open project folder](./04_PVSOL_Photovoltaic_System_Design/)

---

## Skills and tools demonstrated

### CAD and technical drawing

- **AutoCAD:** 2D drafting, layers, line types, symbols, annotations, leaders, legends, and DWG documentation.
- HVAC schematic drafting, including equipment representation, pipe routing, and manifold connections.
- Environmental and civil engineering drawings, including reactor and landfill layouts.

### Energy and building-services simulation

- **GeoT*SOL 2025 R1:** heat pump system configuration and annual performance simulation.
- **PV*SOL 2025:** PV system configuration, module and inverter selection, yield simulation, and financial analysis.
- Interpretation of SPF, PV production, self-consumption, self-sufficiency, grid exports, IRR, and estimated CO₂ avoidance.
- Comparison of scenarios using different locations and household assumptions.

### Environmental and waste engineering

- Municipal waste generation and composition analysis.
- Mass-flow analysis and Sankey diagrams.
- Aerobic stabilization and preliminary reactor sizing.
- Landfill forecasting, capacity and area estimation.
- Wind-rose review and green-belt planning.

### Data, calculations, and documentation

- **Excel:** engineering calculations, forecasting, data organization, and result summaries.
- Technical reporting in Markdown.
- Data-quality review and transparent documentation of source-data limitations.
- Clear statements of project scope, assumptions, and limitations.

---

## Repository structure

```text
04_Engineering-Projects/
├── 01_AutoCAD_Residential_HVAC_Systems_Project/
│   ├── Drawings/        # 3 DWG schematics
│   ├── Previews/        # PNG previews
│   └── README.md
├── 02_Municipal_Waste_Management_Project/
│   ├── Drawings/        # Reactor and landfill basin (DWG)
│   ├── Diagrams/        # Waste-flow diagram
│   ├── Previews/        # PNG previews
│   ├── Source_Files/    # XLSX calculation workbooks
│   ├── Report.md        # Technical report and data-quality review
│   └── README.md
├── 03_GeoTSOL_Heat_Pump_System_Design/
│   ├── 4 simulation reports (PDF)
│   └── README.md
├── 04_PVSOL_Photovoltaic_System_Design/
│   ├── 4 simulation reports (PDF)
│   └── README.md
└── README.md
```

## Notes and limitations

- All projects are educational and portfolio studies, not verified commercial designs or construction documentation.
- GeoT*SOL and PV*SOL results are software simulation outputs based on the assumptions documented in the individual reports. Actual system performance may differ from modeled results.
- The GeoT*SOL reports use the term *geothermal system* in their titles, but the simulated heat source is **ambient air** and the modeled equipment is an **air-to-water heat pump**.
- The 2+4 GeoT*SOL reports use an electricity load profile labelled **1-person household** for the PV-related household load. The 2+4 PV*SOL reports also use a **1-person household** electricity profile. This input limitation should be considered when interpreting the electricity self-consumption and self-sufficiency results.
- The PV*SOL reports were generated using the non-commercial edition of the software.
- Personal names, addresses, company details, and other identifying information shown in the reports are fictional and were created for demonstration purposes.
- Known source-data inconsistencies and modeling limitations are documented in the relevant project reports or notes.

---

**Focus areas:** HVAC · Renewable Energy · Environmental Engineering · AutoCAD  
**Portfolio:** 4 projects · 5 DWG drawings · 8 simulation reports (PDF) · 3 XLSX workbooks
