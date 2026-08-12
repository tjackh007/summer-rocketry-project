# Post-Flight Analysis

## Purpose

Compare the calibrated OpenRocket prediction with what the first real flight can actually support as evidence.

## Prediction vs observation

| Metric | Predicted | Actual / observed | Interpretation |
|---|---:|---:|---|
| Apogee | 203 m | Not measured | No onboard altimeter; cannot quantify error |
| Time to apogee | 7.77 s | Not measured reliably | Video may support future frame-by-frame estimate |
| Maximum velocity | 53.3 m/s | Not measured | Simulation-only value |
| Maximum acceleration | 35.3 m/s² | Not measured | Simulation-only value |
| Recovery deployment | ~7.45 s model event | Parachute visibly deployed | Qualitative agreement |
| Ground-hit velocity | 7.40 m/s | Not instrumented | Recovery was soft enough to cause no damage |
| Final displacement | ~3.38 m | ~6.1 m estimate | Same order of magnitude; actual distance was not surveyed |
| Structural outcome | Nominal model | No damage | Successful qualitative validation |

## What the flight supports

The real flight supports the following conclusions:

1. The as-built rocket had adequate practical stability for the flown configuration.
2. The 1010 rail and F15-4 combination produced a clean departure.
3. Recovery deployment occurred successfully and the 21 in parachute returned the vehicle without damage.
4. The rocket remained recoverable in the actual field/wind conditions.

## What the flight does not prove

Without onboard data, the flight does not validate the predicted 203 m apogee, 53.3 m/s peak velocity, or 35.3 m/s² peak acceleration numerically.

That distinction is intentional. A future flight with an altimeter would be the correct way to turn this qualitative validation into a quantitative model-validation exercise.

## Landing-distance comparison

The model's final simulated displacement was approximately 3.38 m. The observed landing point was estimated at about 20 ft (~6.1 m) from the pad.

Because the actual value was visually estimated and the wind/rail inputs were reconstructed after the flight, a formal percent-error calculation would imply more precision than the evidence supports. The useful conclusion is simply that both model and observation place the rocket very close to the launch area.
