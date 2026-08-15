# Sources and References

## Rocket / manufacturer

- LOC Precision Graduator product page: https://locprecision.com/products/graduator
- LOC entry-level rocket collection retained in project source: https://locprecision.com/collections/rockets-skill-level-entry
- LOC Graduator instructions: [https://cdn.shopify.com/s/files/1/0568/7489/3503/files/PK-16.pdf](https://cdn.shopify.com/s/files/1/0568/7489/3503/files/PK-16-Graduator.pdf?v=1623763227)

## OpenRocket

- https://openrocket.info/

The project preserves the original manufacturer-derived `.ork` baseline separately from the as-built model.

## Motor / hardware

- Estes F15-4 motor configuration selected through the OpenRocket motor database.
- Estes 29 mm retainer, model 24020, identified from manufacturer/vendor specifications supplied during the project.

## Project evidence

- [`data/measurements/kit-baseline.csv`](../data/measurements/kit-baseline.csv)
- [`data/measurements/as-built-summary.csv`](../data/measurements/as-built-summary.csv)
- [`data/measurements/center_of_gravity_measurements.csv`](../data/measurements/center_of_gravity_measurements.csv)
- [`data/open_rocket/simulation-summary.csv`](../data/open_rocket/simulation-summary.csv)
- [`simulations/baseline/LOC_Graduator_manufacturer_baseline.ork`](../simulations/baseline/LOC_Graduator_manufacturer_baseline.ork)
- [`simulations/final_rocket/LOC_Graduator_INSTINCT_as-built_v1.0.ork`](../simulations/final_rocket/LOC_Graduator_INSTINCT_as-built_v1.0.ork)
- [`simulations/exports/data/F15-4_launch-day_conditions.csv`](../simulations/exports/data/F15-4_launch-day_conditions.csv)
- [`simulations/exports/plots/[F15-4]launch-day_flight-plot.png`](../simulations/exports/plots/%5BF15-4%5Dlaunch-day_flight-plot.png)
- [`simulations/exports/screenshots/INSTINCT-final-design-CG-CP.png`](../simulations/exports/screenshots/INSTINCT-final-design-CG-CP.png)
- [`simulations/exports/screenshots/[F15-4]wind-sensitivity-results.png`](../simulations/exports/screenshots/%5BF15-4%5Dwind-sensitivity-results.png)
- [`flight_videos/README.md`](../flight_videos/README.md)

## Evidence hierarchy

For the finished vehicle, measured physical values take precedence over manufacturer model values. Simulation values are clearly identified as predictions and are not substituted for missing flight instrumentation.
