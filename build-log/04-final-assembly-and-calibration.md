# 04 — Final Assembly, Hardware, and As-Built Calibration

## Late July through August 5, 2026

### Rail guidance

The finished rocket uses **two 1010 rail buttons and no launch lug**.

- Aft button installed very near the aft end of the booster.
- Forward button installed exactly **10.00 in (25.4 cm)** forward of the aft button.
- Both buttons aligned on the same axial line.

The change from a generic/older launch-lug representation to the actual 1010 rail-button hardware was reflected in the final OpenRocket model.

### First mass measurement and correction

An initial completed-rocket measurement produced **452 g** without the motor. During final verification, the removable motor-retainer cap was recognized as missing from that weighing.

The rocket was reweighed in the true flight-ready dry configuration:

**Final dry mass = 462 g**

That final number includes the retainer/cap, rail buttons, screws, paint/primer/finish, decals, epoxy/glue, recovery hardware, and other installed flight hardware while excluding the motor and igniter.

Compared with the 412 g manufacturer-model baseline, the completed rocket gained:

- **+50 g**
- **+12.1%**

This was one of the most useful quantitative lessons of the project: a stock model can be geometrically good while still being materially wrong for finished mass properties.

### Center of gravity

The dry CG was measured using a string-loop balance method.

See [`data/measurements/center_of_gravity_measurements.csv`](data/measurements/center_of_gravity_measurements.csv)

- Configuration: complete flight-ready rocket, no motor/igniter
- Independent trials: **5**
- Average CG: **60.5 cm aft of nose tip**
- Measurement/readout uncertainty applied to each trial: **±0.1 cm**
- Sample standard deviation: **0.77 cm**
- Standard error of the mean: **0.34 cm**

The ±0.1 cm value represents the assumed measurement resolution/reading uncertainty and is distinct from the observed trial-to-trial spread.

This measured value replaced the OpenRocket-estimated dry CG through a stage-level mass/CG override.

### Final OpenRocket calibration

The final as-built model incorporated:

- 462 g dry stage mass override
- 60.5 cm dry CG override
- Estes 29 mm retainer representation
- two 1010 rail buttons
- no launch lug
- Estes F15-4 motor configuration

With the F15-4 loaded, OpenRocket displayed approximately:

- Loaded mass: 565 g
- Loaded CG: 66.5 cm
- CP: 81.2 cm
- Stability: 2.21 calibers

At this point the model represented the physical rocket closely enough for launch-day simulation work.
