# Exporting CAN Signal Data (View-Only Mode - Conceptual)

In a fully licensed version of CANalyzer, signals can be exported via:
- **Trace Window** → Export messages
- **Data/Graphics Window** → Export signal trends to `.csv` or `.mat`

However, in the **View-Only mode**, export functions are **disabled**, as shown below:

Screenshot: `Step3_Export_Button_Disabled_ViewOnly.png`

## Conceptual Steps (If Export Were Enabled):
1. **Right-click** in Trace or Data window.
2. Select **Export** → Choose format (`CSV`, `TXT`, `MAT`).
3. Choose **time range** and **signals** to export.
4. Open the exported file in Excel/MATLAB.
5. Plot the signal vs time for visual analysis.

**Note**: This project uses mock export data (`mock_export.csv`) and a sample chart (`excel_plot.png`) to demonstrate how exports are handled in licensed mode.
