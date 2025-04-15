## Filters Applied in Trace Window

In this mini project, various filters were applied to the Trace Window using the **Filter Configuration Panel**.

---

## Message IDs Passed Through
The following CAN IDs were configured as **active** and passed through:

- **0x600**
- **0x700**
- **0x601**
- **0x701**

These were mapped on **CAN Channel 1** and **CAN Channel 2** (as seen in the filter block).

---

## Filter Logic

- **Pass Filter** was applied to only allow selected messages to pass.
- Data Field was set to: `Ignore` (to reduce noise).
- Filters were activated from:  
  `Filter > CAN Filter Block 3`

---

## Observations:

- IDs like `0x600` and `0x700` are commonly used in demo setups to simulate real vehicle messages.
- All filtered frames showed up as `<Unknown Frame>` in View-Only mode due to license restriction (no decoding).
- Despite this, the Trace Window successfully displayed raw message flow and DLC, aiding in frame-level debugging.

---

## Screenshot Reference:
Refer to `Step4_TraceWindow_FilterConfig_ViewOnly.png` for visual configuration proof.
