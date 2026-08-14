# Lessons Learned

## 1. The finished rocket is the source of truth

The manufacturer model predicted a 412 g dry rocket. The completed vehicle was 462 g — a **12.1% increase**. Paint, primer, epoxy, hardware, screws, rail buttons, and motor retention are individually small but collectively meaningful.

## 2. Reweigh the exact flight configuration

The first final mass measurement was 452 g because the motor-retainer cap was accidentally omitted. Catching that mistake and updating the model to 462 g was a better engineering outcome than keeping the earlier number for consistency.

## 3. Measure CG rather than trusting component bookkeeping

The five-trial string balance provided a defensible 60.5 cm dry CG and avoided trying to estimate the position of every gram of adhesive and finish.

## 4. Model the actual launcher

A placeholder 1 m launch-guide value materially changed rail-exit interpretation. Reconstructing the actual ~10 ft 1010 rail and using ~2.75 m effective guidance made the simulation more representative.

## 5. Wind sensitivity is more useful than one “perfect” simulation

The wind matrix showed a consistent trend: higher wind reduced apogee and increased deployment/landing velocity. This gave a better picture of robustness than a single nominal run.

## 6. Preserve warnings instead of gaming them away

The body-diameter discontinuity warning was informational. It was recorded rather than changing the model only to make the software look clean.

## 7. Field readiness includes mundane fit checks

A small fit issue required a tape adjustment at the field. A complete pre-field assembly check — including motor/retainer/recovery/rail interface — is worth doing even when the rocket is “finished.”

## 8. Flight video can provide useful validation even without onboard telemetry

Although no altimeter or flight computer was carried, post-flight video timestamp analysis provided an estimated 7.82 s time from liftoff to apogee. The launch-day OpenRocket model predicted 7.77 s, a difference of approximately 0.05 s (~0.6%).

Recovery-system deployment was also observed immediately before apogee, consistent with the model's predicted near-apogee deployment timing.

This provided meaningful quantitative validation of ascent timing in addition to the qualitative observations of trajectory and recovery behavior. However, video analysis cannot replace onboard instrumentation for measurements such as actual apogee altitude, velocity, acceleration, or a complete flight time history. A future flight carrying an altimeter or flight computer would allow these parameters to be compared directly against the OpenRocket model.
