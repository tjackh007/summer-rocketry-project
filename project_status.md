# Project Status

## Final status

**COMPLETE / FLIGHT TESTED — August 2026**

| Work item | Status | Evidence |
|---|---|---|
| Project definition / rocket selection | Complete | `docs/project-overview.md` |
| Manufacturer OpenRocket baseline | Complete | `openrocket/baseline/` |
| Kit inventory / pre-build measurements | Complete | `photos/kit-inventory/`, `data/measurements/kit-baseline.csv` |
| Physical build / finishing | Complete | Build log |
| Motor retainer | Complete | Estes 29 mm model 24020 documented |
| Two 1010 rail buttons | Complete | 10 in center-to-center; no launch lug |
| Final dry mass | Complete | 462 g |
| Final dry CG | Complete | 60.5 cm, 5-trial average |
| As-built OpenRocket calibration | Complete | Final screenshots / local `.ork` |
| F15-4 wind sensitivity | Complete | `data/simulations/simulation-summary.csv` |
| Launch-day reconstruction | Complete | Raw export + plot |
| Flight | Complete | August 8, 2026 |
| Recovery | Complete | Successful; ~20 ft from pad; no damage |
| Post-flight analysis | Complete | Qualitative due to no onboard altimeter |
| Final GitHub documentation | Complete | This repository package |

## Manual publishing check

Before calling the GitHub repository fully archived:

- [ ] Copy `LOC_Graduator_INSTINCT_as-built_v1.0.ork` into `openrocket/final/`.
- [ ] Add a favorite finished-rocket photograph to `photos/build/` and optionally make it the README hero image.
- [ ] Add launch/recovery video clips only if desired; use compressed clips or Git LFS for large files.
- [ ] Run `python scripts/verify_repository.py`.
- [ ] Commit and push.
- [ ] Create Git tag/release `v1.0-flight-tested`.
