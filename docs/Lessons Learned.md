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

## 8. Instrumentation would improve the next iteration

The project successfully validated launch and recovery qualitatively, but an altimeter would allow actual apogee and time-history data to be compared directly with OpenRocket.
