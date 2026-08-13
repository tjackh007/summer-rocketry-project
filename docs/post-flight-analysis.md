# Post-Flight Analysis

## Purpose

Compare the calibrated OpenRocket prediction with what the first real flight can actually support as evidence.

## Prediction vs observation

| Metric | Predicted | Actual / observed | Interpretation |
|---|---:|---:|---|
| Apogee | 203 m | Not measured | No onboard altimeter; cannot quantify error |
| Time to apogee | 7.77 s | ~7.82 s from video timestamp analysis | +0.05 s difference (~0.6%); strong agreement within video measurement limitations |
| Recovery deployment | ~7.45 s model event | Observed immediately before apogee | Qualitative agreement with predicted near-apogee deployment |
| Maximum velocity | 53.3 m/s | Not measured | Simulation-only value |
| Maximum acceleration | 35.3 m/s² | Not measured | Simulation-only value |
| Ground-hit velocity | 7.40 m/s | Not instrumented | Recovery was soft enough to cause no damage |
| Final displacement | ~3.38 m | ~6.1 m estimate | Same order of magnitude; actual distance was not surveyed |
| Structural outcome | Nominal model | No damage | Successful qualitative validation |

## Video-Derived Flight Timing

Post-flight review of the launch video was used to estimate the elapsed time from liftoff to apogee. Based on video timestamp analysis, the observed time to apogee was approximately **7.82 s**.

The reconstructed launch-day OpenRocket model predicted apogee at **7.77 s**, producing a difference of approximately **0.05 s**, or about **0.6%** relative to the simulation prediction.

The video also shows recovery-system deployment beginning immediately before apogee. This behavior is consistent with the OpenRocket launch-day model, which predicted motor ejection at approximately **7.45 s** and apogee at approximately **7.77 s**.

Because this measurement was derived from video rather than onboard instrumentation, it should not be treated as equivalent to altimeter or flight-computer telemetry. However, it provides useful quantitative evidence that the modeled ascent timing closely matched the observed flight.

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
