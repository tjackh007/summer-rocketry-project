# OpenRocket Simulation Analysis

## Model basis

All final cases use the same calibrated as-built rocket:

- Dry mass: 462 g
- Dry CG: 60.5 cm aft of nose
- Motor: Estes F15-4
- Launch guide: 1010 rail
- Effective rail length: approximately 2.75 m

The sensitivity exercise intentionally varies wind while holding the vehicle configuration constant.

## Results

| Scenario | Rail exit | Apogee | Deployment velocity | Optimum delay | Max velocity | Max acceleration | Time to apogee | Flight time | Ground-hit velocity |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Calm | 12.1 m/s | 216 m | 7.11 m/s | 4.72 s | 53.5 m/s | 35.3 m/s² | 7.99 s | 39.4 s | 6.95 m/s |
| Light wind | 12.1 m/s | 212 m | 9.27 m/s | 4.72 s | 53.4 m/s | 35.3 m/s² | 7.89 s | 38.8 s | 7.17 m/s |
| Nominal wind | 12.1 m/s | 201 m | 13.6 m/s | 4.47 s | 53.3 m/s | 35.3 m/s² | 7.75 s | 37.1 s | 7.57 m/s |
| High wind | 12.1 m/s | 184 m | 17.8 m/s | 4.17 s | 53.0 m/s | 35.3 m/s² | 7.58 s | 34.6 s | 8.67 m/s |
| Launch day | 12.1 m/s | 203 m | 13.0 m/s | 4.52 s | 53.3 m/s | 35.3 m/s² | 7.77 s | 37.4 s | 7.40 m/s |

[`Wind Sensitivity Results`](simulations/exports/screenshots/[F15-4]wind-sensitivity-results.png)

## Interpretation

### Rail departure

Rail-exit velocity remained approximately 12.1 m/s in each case because the rocket/motor/rail geometry was unchanged. The longer real 1010 rail was important: early placeholder simulations using a 1 m guide were not representative of the actual launcher.

### Apogee

Predicted apogee declined from 216 m in calm conditions to 184 m in the high-wind sensitivity case. The reconstructed launch-day prediction was 203 m.

### Recovery timing

The F15-4 fixed delay was reasonably close to the modeled optimum across all cases. Launch day predicted:

- Motor burnout: ~3.45 s
- Ejection: ~7.45 s
- Apogee: ~7.77 s
- Optimum delay: 4.52 s

Thus the modeled recovery event occurred about **0.32 s before apogee**.

### Recovery loading

The largest wind-related change was deployment velocity. It increased from 7.11 m/s in calm conditions to 17.8 m/s in the high-wind case. This was a more useful launch-planning indicator than apogee alone.

### OpenRocket warning

The final simulations retained one informational message:

> Discontinuity in rocket body diameter: "Nose cone", "Body tube"

The warning was documented rather than eliminated by changing geometry solely to satisfy the software.

## Raw data

The launch-day time history is retained in both spreadsheet and CSV form:

- `openrocket/exports/data/F15-4_launch-day_conditions.xlsx`
- `openrocket/exports/data/F15-4_launch-day_conditions.csv`

The CSV contains 356 simulated data points and 14 exported variables, including altitude, velocity, acceleration, lateral motion, angle of attack, CG location, stability, and wind.
