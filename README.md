# CANalyzer-Restricted-Learning

This repository showcases my **project-based learning using Vector CANalyzer** under a **restricted View-Only license**. Despite tool limitations, I explored essential panels and simulated core validation workflows through hands-on mini-projects.

---

## Objective

To gain practical experience in:
- CAN message decoding via DBC
- Trace and Data window navigation
- Signal filtering, export logic, and graphical visualization

---

## Tool: Vector CANalyzer (View-Only Mode)

- DBC: `motbus.dbc`
- Config: `CANMainDemo.cfg`
- Simulation Mode: Offline & View-Only

---

## Mini Projects Summary

### MiniProject 1: CAN Log Decoder
Loaded `.blf` log file  
Added and verified DBC mapping  
Extracted signals: `CarSpeed`, `EngSpeed`, `IdleRunning`  
[`decoded_signals_summary.md`](MiniProject-1_CAN-Log-Decoder/decoded_signals_summary.md)  
Screenshot: `Step4_DBC_Loaded_ViewOnly.png`

---

### MiniProject 2: Trace Debug Walkthrough
Applied ID filters in Trace  
Analyzed unknown frames and routing  
[`filters_applied.md`](MiniProject-2_Trace-Debug/filters_applied.md)  
Screenshot: `Step4_TraceWindow_FilterConfig_ViewOnly.png`

---

### MiniProject 3: Signal Viewer
Tagged signals as favorite  
Viewed `CarSpeed`, `Gear`, `EngSpeed` in Data + Graphics Window  
[`analysis_notes.md`](MiniProject-3_Signal-Viewer/analysis_notes.md)  
`Step5_DataWindow_SignalTagging_Favorites_ViewOnly.png`,  
`Step6_GraphicsPanel_SignalCurves_Configured_ViewOnly.png`

---

### MiniProject 4: Simulated Export + Excel Plot
Created mock `.csv` of signal data  
Plotted signal behavior using Excel  
[`export_steps.md`](MiniProject-4_Export-Plan/export_steps.md)  
[`mock_export.csv`](MiniProject-4_Export-Plan/mock_export.csv) | [`excel_plot.png`](MiniProject-4_Export-Plan/excel_plot.png)  
`Step5_Graphics_Export_Disabled_ViewOnly.png`,  
`Step3_Export_Button_Disabled_ViewOnly.png`

---

### Extras

[`Extras/`](Extras): Contains general CANalyzer tool UI visuals  
- Offline mode setup  
- Statistics and trace views  
- Dashboard & simulation panels  
- Startup interface  
- Unmapped/mapped log configurations

---

## Key Learnings
- CAN signal decoding and message exploration  
- Interface familiarity: Trace, Data, Graphics, Filters  
- Export workflows even under restricted conditions  
- DBC structure understanding via CANdb++  
