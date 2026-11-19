# Adaptive LDO Regulator for Wearable ECG Systems

![Proposed LDO](images/Proposed%20LDO.jpeg)

Simulation assets for an adaptive low-noise low-dropout regulator designed for wearable ECG applications.

## Overview

The design combines:

- A low-quiescent-current DC feedback path
- An AC-coupled dynamic current booster for fast load transients
- Adaptive biasing of the error amplifier
- An on-chip bandgap reference

The objective is to maintain a regulated 3 V output while limiting standby quiescent current and improving transient recovery.

## Repository Contents

```text
adaptive-ldo-ecg-regulator/
|-- images/
|-- docs/
|   `-- results.md
|-- README.md
`-- .gitignore
```

## Key Highlights

- Nominal output voltage: 3.0 V
- Bandgap reference: approximately 1.20 V
- DC load regulation: approximately 0.048 mV/mA
- Phase margin across tested load conditions: above 62 degrees
- Adaptive quiescent-current operation from standby to higher load conditions
- Load and supply transient characterization

## Design Assets

### Schematics

- [Bandgap reference](images/BGR_Schematic.png)
- [Error amplifier](images/OpAmpwoadap_Schematic.png)
- [Adaptive error amplifier](images/OpAmpadap_Schematic.png)
- [Dynamic current booster](images/DCB_Schematic.png)
- [Adaptive LDO](images/LDOadp_Schematic.png)
- [Complete transistor-level schematic](images/transistor%20level%20schematic.png)

### Characterization

- [Quiescent current vs. load](images/adaptive_LDO_IloadvsIQ.png)
- [Adaptive amplifier current](images/adaptive_Opamp_IloadvsIQ.png)
- [Load regulation](images/load_reg_dc_sweep_merged.png)
- [Line regulation](images/line_reg_dc_sweep.png)
- [Dynamic-load response](images/load_reg_with_dcb.png)
- [PSRR without load](images/psrr_no_load.png)

See [results.md](docs/results.md) for a concise summary of the recorded measurements.
