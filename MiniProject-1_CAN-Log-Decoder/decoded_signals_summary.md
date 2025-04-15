# Decoded Signals Summary

This summary lists the signals observed in the Data/Trace Windows and maps them to their likely CAN message IDs. These signals were decoded using a `.dbc` file (`motbus.dbc`) loaded in View-Only Mode.

---

## Signals Decoded

| Signal Name                    | Unit     | Description                             | Expected Range | Observations                  |
|--------------------------------|----------|----------------------------------------|----------------|-------------------------------|
| `CarSpeed`                     | km/h     | Vehicle speed                          | 0–250          | Standard motion range         |
| `EngSpeed`                     | rpm      | Engine revolutions per minute          | 0–8000         | High refresh rate, real-time  |
| `EngTemp`                      | °C       | Engine temperature                     | 0–150          | Slowly rising during warm-up  |
| `WheelInfoIEEE::WheelSpeedFL`  | 1/min    | Front-left wheel rotation speed        | 0–300          | Similar pattern to CarSpeed   |
| `IdleRunning`                  | (bool)   | Engine idle state (ON/OFF)             | 0/1 (binary)   | Tied to throttle/off-pedal    |
| `Gear`                         | number   | Gear level                             | 0–6            | Mapped to graphical dashboard |

---

## Message IDs (from Trace Filter Config)

| CAN ID   | Likely Signals                     | Channel |
|----------|------------------------------------|---------|
| `0x600`  | `EngSpeed`, `EngTemp`              | 1       |
| `0x601`  | `CarSpeed`, `Gear`                 | 1       |
| `0x701`  | `IdleRunning`, `WheelSpeedFL`      | 2       |

*Note: Message ID to signal mapping is assumed from standard DBC structures and naming conventions.*

---

##Cycle Time (Assumed)

Due to View-Only Mode, cycle time was not directly measured. Based on signal nature:

- `CarSpeed`, `EngSpeed` → ~10–20 ms (high-frequency updates)
- `EngTemp` → ~500 ms (slow thermal change)
- `Gear`, `IdleRunning` → ~100 ms (event-based or periodic)
- `WheelSpeedFL` → ~20–50 ms

---

##Additional Notes

- Signal tagging was enabled via the **Favorites column** in the Data Window.
- These signals were tracked visually in Data and Graphics panels.
- The simulation was based on `Logging.blf` loaded via Offline Mode and `motbus.dbc`.

---

**Next Step:** Use this decoded mapping to apply filters, visualize signals in Graphics Window, or simulate export.
