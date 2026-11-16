# PMSM Drive Model in MATLAB/Simulink, Validated on Hardware

**Status: in progress.** This repository is being built; nothing here is a finished result yet.

## Goal

A MATLAB/Simulink model of a PMSM drive: identify Rs, Ld/Lq and flux linkage by bench tests, tune the current and speed loops by pole placement, validate model against hardware steps, map efficiency over operating points and compare SVPWM with sine PWM.

## Layout

```
matlab/params/            # Motor and inverter parameter files.
matlab/build/             # Scripts that build the Simulink model (logic kept in .m, not only .slx).
matlab/control/           # PI design by pole placement.
param-id/                 # Bench test procedures and scripts for parameter identification.
param-id/data/            # Raw bench logs.
validation/               # Model vs hardware step comparisons.
efficiency/               # Operating-point sweep and efficiency maps.
docs/                     # Method and results.
```

## Plan

- [ ] Parameter files and model build scripts
- [ ] Bench parameter identification
- [ ] Loop tuning by pole placement
- [ ] Model vs hardware validation
- [ ] Efficiency map
- [ ] SVPWM vs sine PWM comparison
- [ ] Write-up
