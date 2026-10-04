# Print Settings – Fixed Proximity Sensor Bracket

## 1. Overview

This document records the Cura slicing settings used for the fixed-position proximity sensor bracket.

The source profile was exported from Ultimaker Cura using a Creality Ender-3 family printer definition. The `.curaprofile` is a differential profile, meaning it only contains settings that were changed from Cura's underlying **Standard** quality profile. Any setting not listed here remains inherited from that base profile.

---

## 2. Printer / Profile

| Parameter | Setting |
|---|---|
| Printer definition | Creality base / Ender-3 family |
| Cura profile name | TEST_SPEED |
| Quality profile | Standard |
| Profile type | Quality Changes |
| Setting version | 25 |

---

## 3. Layer Settings

| Parameter | Setting |
|---|---|
| Adaptive layers | Enabled |
| Base layer height | Inherited from Standard profile |
| Adaptive layer parameters | Inherited from Standard profile |

---

## 4. Material / Temperature

| Parameter | Setting |
|---|---:|
| Bed temperature | 85 °C |
| Nozzle temperature | Inherited from material / Standard profile |

---

## 5. Print Speeds

| Parameter | Setting |
|---|---:|
| General print speed | 60 mm/s |
| Infill speed | 90 mm/s |
| Outer wall speed | 35 mm/s |
| Inner wall speed | 60 mm/s |
| Top / bottom speed | 35 mm/s |
| Travel speed | 200 mm/s |

---

## 6. Acceleration

Acceleration control is enabled.

| Parameter | Setting |
|---|---:|
| General print acceleration | 1000 mm/s² |
| Wall acceleration | 750 mm/s² |
| Infill acceleration | 2000 mm/s² |
| Travel acceleration | 2250 mm/s² |

---

## 7. Jerk

Jerk control is enabled.

| Parameter | Setting |
|---|---:|
| Travel jerk | 12 mm/s |
| Other jerk values | Inherited from Standard profile |

---

## 8. Infill

| Parameter | Setting |
|---|---|
| Infill density | 10% |
| Infill pattern | Lines |
| Infill speed | 90 mm/s |

---

## 9. Supports

| Parameter | Setting |
|---|---|
| Supports | Disabled |
| Selected support structure | Tree |

Tree supports are selected in the profile but are inactive because support generation is disabled.

---

## 10. Build Plate Adhesion

| Parameter | Setting |
|---|---|
| Build plate adhesion | None |

No brim, raft, or skirt override is stored in the exported profile.

---

## 11. Design-for-Manufacture Notes

The bracket should be oriented so that:

- Support material is not required.
- The largest practical flat surface contacts the build plate.
- Layer orientation provides adequate strength around the sensor mounting feature and machine mounting holes.
- Critical holes and sensor-fitting features can be inspected after printing.
- The M18 sensor bore can be adjusted in a later revision if dimensional testing identifies insufficient clearance.

---

## 12. Post-Print Inspection

After manufacture, verify:

| Feature | Check |
|---|---|
| Sensor bore | M18 proximity sensor fits correctly |
| Mounting holes | Fasteners fit without excessive clearance |
| Mounting face | Sits flat against intended surface |
| Bracket rigidity | No excessive flexing during installation |
| Sensor retention | Sensor remains securely fixed |
| Surface / layer quality | No defects affecting function |

Any dimensional or functional issues identified during testing should be recorded and incorporated into the next design revision.

---

## 13. Settings Not Explicitly Included in the Export

The following values were not overridden in the supplied Cura profile and therefore remain dependent on the selected Cura printer, material, and Standard quality profiles:

- Nozzle temperature
- Layer height
- Initial layer height
- Wall line count
- Top / bottom layer count
- Retraction settings
- Cooling / fan settings
- Flow rate
- Line width
- Initial layer speed
- Remaining acceleration values
- Remaining jerk values

These values should be recorded separately if a fully reproducible manufacturing specification is required.
