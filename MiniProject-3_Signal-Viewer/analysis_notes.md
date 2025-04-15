# MiniProject 3: Signal Viewer – Analysis Notes

## Overview
This project visualizes decoded CAN signals on the **Graphics Panel** in Vector CANalyzer (View-Only Mode). Although real-time updates are not possible, the panel setup simulates how engineers track signal behavior during driving or test simulations.

---

## Signals Tracked
| Signal Name | Unit      | Description                  | Visual Cue     |
|-------------|-----------|------------------------------|----------------|
| EngSpeed    | rpm       | Engine speed, scaled 0–8000  | Blue axis      |
| CarSpeed    | km/h      | Vehicle speed, scaled 0–250  | Red axis       |
| Gear        | gear pos. | Gear state (0–5), discrete   | Green text line|

---

## Insights
- **Gear shifting** is clearly visible as a step-wise signal on the green line, switching from Idle to Gear 1–5.
- **CarSpeed and EngSpeed** are continuous variables showing ramp-up and down patterns.
- These signals align well on the time scale (X-axis), supporting time-based diagnosis.
- Axis scaling was adjusted manually in **Graphic Configuration > Symbols/Axes** to improve visibility.

---

## Purpose
Helps validation engineers correlate signal behavior with driver actions (gear change, acceleration) and check for anomalies in real-time or simulated playback.

---

> Note: Graph behavior in this setup is static due to View-Only restrictions, but panel configuration reflects typical industry usage.
