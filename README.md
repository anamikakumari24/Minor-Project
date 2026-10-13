# Thermohydraulic Performance of Plain Twisted Tape Inserts with Oxide Nanofluids in Turbulent Tube Flow

**Minor Project (Semester 4) · Department of Mechanical Engineering, NIT Jamshedpur**

An experimental study of whether a *simple* plain twisted tape (TT) combined with a *high-conductivity nanofluid* can match the performance of a more *complex* hyperbolic-cut twisted tape (HCTT) running on plain water.

---

**Supervisor:** Dr. Laljee Prasad
**Institute:** National Institute of Technology Jamshedpur

---

## Overview

Twisted tape inserts are a passive heat-transfer enhancement technique: they create swirl, disturb the boundary layer and improve mixing, but at the cost of higher pressure drop. Nanofluids offer a second route by raising the thermal conductivity of the working fluid.

This project combines both approaches and compares three oxide nanofluids under identical experimental conditions across different twist ratios. The results are benchmarked against the HCTT + water data of the base paper (Rajan et al., 2025).

## Objectives

1. Investigate the thermohydraulic performance of plain twisted tape inserts in turbulent tube flow.
2. Compare **GO/water**, **CuO/water** and **Al₂O₃/water** as working fluids.
3. Study the effect of twist ratios **2, 3 and 4** on heat transfer and friction.
4. Evaluate the effect of Reynolds number and nanoparticle concentration.

---

## Experimental Setup

| Parameter | Value |
|---|---|
| Test section | Galvanised iron (GI) tube |
| Tube length (L) | 800 mm |
| Tube inner diameter (D) | 20 mm |
| Tape material | GI sheet |
| Tape width (w) / thickness (t) | 18 mm / 2 mm |
| Twist ratio (TR = y/w) | 2, 3, 4 |
| Pitch (y) | 36, 54, 72 mm |
| Heating | Nichrome wire (46 Ω, 1.5 kW) with variable transformer, uniform heating |
| Insulation | 30 mm glass wool wrapped in aluminium foil |
| Reynolds number range | 10,000 – 22,000 (turbulent) |

**Instrumentation**

- 7 × K-type thermocouples along the tube (wall temperature)
- RTD Pt-100 sensors at inlet and outlet (accuracy 0.1 °C)
- U-tube manometer for pressure drop (accuracy 2 Pa)
- Calibrated rotameter for flow rate (accuracy 0.3%)
- Two-point calibration; readings taken after at least 10 minutes of steady state

**Nanofluids**

- Fluids: Water, GO/water, CuO/water, Al₂O₃/water
- Volume concentrations: 0.1%, 0.3%, 0.5%
- Preparation: two-step method, 90 min ultrasonication; sodium dodecyl sulphate (SDS) added as surfactant to two of the fluids
- Properties (density, specific heat, viscosity, thermal conductivity) evaluated at 25 °C

---

## Data Reduction

| Quantity | Expression |
|---|---|
| Heat transfer rate | Qc = ṁ · Cp · (To − Ti) |
| Heat transfer coefficient | h = Qc / (T̄w − Tb), with Tb = (Ti + To)/2 |
| Nusselt number | Nu = h · D / k |
| Friction factor | ΔP = f · (L/D) · (½ρV²) |
| Thermohydraulic performance | η = (Nu/Nup) / (f/fp)^(1/3) |

Nup and fp are the plain-tube values from the Dittus–Boelter and Blasius correlations. Nanofluid properties are used in all calculations.

**Validation:** the plain tube agrees with Dittus–Boelter within ±5.86% and with Blasius within ±4.72%. Plain TT (TR = 3, water) agrees with Mangal et al. (2013) within ±6.1%.

---

## Key Results

### Nanofluid ranking (Nusselt number enhancement over the water baseline)

| Nanofluid | Approx. Nu enhancement |
|---|---|
| **GO/water** | **~34%** |
| CuO/water | ~27% |
| Al₂O₃/water | ~22% |

The ranking GO > CuO > Al₂O₃ held across all tested Reynolds numbers and concentrations. It reflects the higher effective thermal conductivity of graphene oxide. Higher concentration (0.5%) gives higher Nu, but also higher viscosity and pressure drop.

### Effect of twist ratio

- Lower TR gives higher Nu and higher friction factor because of stronger swirl.
- With water, TR = 2 gives about 18.3% higher Nu than TR = 4 (at Re = 22,000).
- **TR = 3** is the best compromise for water (η ≈ 1.09–1.14).
- Optimum TR depends on the fluid: **TR = 3** for GO/water (η ≈ 1.19–1.23); **TR = 2** for CuO/water (η ≈ 1.15–1.18) and Al₂O₃/water (η ≈ 1.13–1.16).

### Comparison with the base paper (η vs Reynolds number)

| Configuration | Re = 10,000 | Re = 16,000 | Re = 22,000 |
|---|---|---|---|
| Plain TT, water, TR = 3 | ~1.04 | ~1.02 | ~1.00 |
| Plain TT, GO/water 0.5%, TR = 3 | ~1.21 | ~1.18 | ~1.15 |
| Plain TT, CuO/water 0.5%, TR = 2 | ~1.18 | ~1.15 | ~1.11 |
| Plain TT, Al₂O₃/water 0.5%, TR = 2 | ~1.16 | ~1.13 | ~1.09 |
| HCTT, water (Rajan et al., 2025) | 1.165 | ~1.12 | 1.060 |

## Conclusion

A simple twisted tape with GO/water nanofluid achieves thermohydraulic performance comparable to, or slightly better than, the more complex HCTT with plain water. This suggests a possible route to simpler, easier-to-manufacture heat exchanger tubes, with the caveat that the cost and stability of preparing and maintaining nanofluids must also be considered.

---

## Repository Contents

```
├── Report_Minor.pdf    # Full project report
├── PPT_Minor.pptx      # Project presentation
└── README.md
```

## References

1. Rajan A. et al. (2025), *Multiscale and Multidisciplinary Modeling, Experiments and Design* 8:384
2. Rajan A., Prasad L. (2022), *Proc. IMechE Part C: J. Mech. Eng. Sci.*
3. Rajan A., Prasad L. (2021), *Energy Sources Part A*
4. Eiamsa-ard S. et al. (2010), *Int. Commun. Heat Mass Transf.* 37(1):39–46
5. Mangal S.K. et al. (2013), *Exp. Thermal Fluid Sci.* 46:160–166
6. Sundar L.S., Singh M.K. (2013), *Int. Commun. Heat Mass Transf.* 44:41–47
7. Heyhat M.M. et al. (2013), *Exp. Thermal Fluid Sci.* 44:520–527

The full reference list is in the report.

## Acknowledgement

We thank Dr. Laljee Prasad for his supervision and guidance, the Head of the Department of Mechanical Engineering for providing institutional resources, and the faculty of the department for their support.
