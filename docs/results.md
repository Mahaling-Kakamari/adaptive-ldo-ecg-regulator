# Recorded Simulation Results

## DC and Reference

| Parameter | Recorded result |
|---|---:|
| Bandgap reference | approximately 1.200 V |
| Bandgap temperature drift | approximately 4.5 mV from -40 to +125 C |
| Nominal output voltage | approximately 3.000 V |
| DC load regulation | approximately 0.048 mV/mA |

## Stability

| Load | Unity-gain frequency | Phase margin | Gain margin |
|---|---:|---:|---:|
| 10 uA | 61.62 kHz | 71.92 deg | 47.41 dB |
| 1 mA | 1.52 MHz | 65.76 deg | 19.39 dB |
| 5 mA | 4.41 MHz | 62.60 deg | 12.18 dB |

## Power

The recorded standby and load-dependent quiescent-current behavior is shown in:

- `adaptive_LDO_IloadvsIQ.png`
- `adaptive_Opamp_IloadvsIQ.png`

## Additional Plots

- Supply and temperature response of the bandgap reference
- DC load and line regulation
- Dynamic-current-booster step responses
- PSRR under multiple load conditions
