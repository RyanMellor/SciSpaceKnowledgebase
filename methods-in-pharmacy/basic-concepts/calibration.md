---
description: General method for determining the concentration of a substance in a sample
---

# Calibration

## Calibration Curve

A calibration curve is a plot of **responses** from standards of **known concentrations** against those concentrations. **Unknown concentrations** can be determined by comparing the response to the calibration curve.

Most techniques will produce a linear response, with respect to concentration, within an appropriate range. The [dynamic range ](validation.md#dynamic-range)is dependent on the technique and the analyte.

### Procedure

10-fold serial dilutions (repeated dilution of 1 part standard in 9 parts solvent) can be used for scouting the [dynamic range](validation.md#dynamic-range) but should not be used as the final curve as higher concentrations will have greater leverage over the line equation.

A good calibration curve should cover 25-200% of the target concentration, it may be necessary to dilute samples to fall into an appropriate range for the instrument, this is not a problem as long as the dilution factor is taken into consideration.

Prepare and analyse, in triplicate, standard solutions at six concentrations, typically 25, 50, 75, 100, 150, and 200%.

Plot the concentration (x-axis) against response (y-axis). Calculate the [straight line equation](data-analysis.md#linear-regression), and[ $$r^2$$](data-analysis.md#coefficient-of-determination)value. See [validation ](validation.md)for more detail on assay validation.

## Matrix Effect

Matrix effect (ME) is the contribution of non-analyte components to the response. Matrix effect can be significant if the matrix affects properties of the sample important to the analysis, e.g. viscosity, ionic strength, or if the responses overlap. Closely related are recovery from extraction (RE) and process efficiency (PE).

$$ME = 100(\frac{A_{spike}}{A_{standard}})$$

$$RE = 100(\frac{A_{process}}{A_{spike}})$$

$$PE = 100(\frac{A_{process}}{A_{standard}})$$

Where:

* $$A_{standard}$$ = Response from analyte without matrix present
* $$A_{spike}$$ = Response from analyte with matrix present
* $$A_{process}$$ = Response from analyte processed with matrix

$$ME < 100$$: suppression

$$ME ≈ 100$$: no matrix effect

$$ME > 100$$: enhancement

![](<../../.gitbook/assets/Extraction standards (2).png>)

## Internal Standard

An internal standard is a compound added in a constant amount to all samples including blanks and standards, the calibration curve is then constructed from the ratio of the two responses against the analyte concentration.

Internal standards are used to account for analyte loss during processing. The compound should be as similar to the analyte as possible - to ensure similar recovery, response, and derivatization - while still being readily distinguishable by the instrument. The internal standard should have no possibility of occurring in the sample before its addition, e.g. no degradation products.
