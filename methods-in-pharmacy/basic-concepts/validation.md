---
description: >-
  Process used to confirm that the analytical procedure is suitable for its
  intended use
---

# Validation

### Accuracy

**Definition:** The closeness of an assay value to the true value

**Procedure:** Prepare, in triplicate, standard solutions at three concentrations, typically 50, 100, and 150% of target concentration.

**Analysis and acceptance:** Calculate the mean, standard deviation, RSD, and % recovery ($$100\left(\frac{assay\ value}{theoretical\ value}\right)$$) for each sample. Accept if the mean % recovery for each concentration is in the acceptable range, $$\pm10\%$$ for non-regulated products,  $$\pm2\%$$ for dosage forms, and  $$\pm1\%$$ for drug substance.

### Dynamic Range

**Definition:** The range of analyte concentration over which the response is [linear](validation.md#linearity). Extends from the [limit of detection](validation.md#limit-of-detection) to the concentration where the response deviates from linearity.

### Intermediate Precision

**Definition:** The [precision ](validation.md#precision)obtained in a single lab over a period of time (typically months) with introduced variability, e.g. different analyst, instrument, or chemical batch.

**Procedure:** The same analysis will be performed by two analysts, using two instruments, on different days. Analysis will be performed on standard solutions at three concentrations, typically 50, 100, and 150% of target concentration.

**Analysis and acceptance:** Calculate the mean, standard deviation, and RSD for analysts and instruments. Accept if RSD $$\leq2\%$$.

### Limit of Detection (LoD)

**Definition:** The smallest concentration of analyte an assay can reliably distinguish from zero. Determined from the calibration curve.

$$LoD = 3.3\left(\frac{S_{y,x}}{m}\right)$$

Where:

* $$S_{y,x}$$ = [Standard error of the predicted y-value](data-analysis.md#standard-error-of-the-predicted-y-value)
* $$m$$ = [Slope](data-analysis.md#linear-regression)

### Limit of Quantification (LoQ)

**Definition:** The smallest concentration of analyte an assay can reliably determine with acceptable [repeatability](validation.md#precision-repeatability). Determined from the calibration curve.

$$LoQ = 10\left(\frac{S_{y,x}}{m}\right)$$

Where:

* $$S_{y,x}$$ = [Standard error of the predicted y-value](data-analysis.md#standard-error-of-the-predicted-y-value)
* $$m$$ = [Slope](data-analysis.md#linear-regression)

### Linearity

**Definition:** The property of a data set to fit a straight line plot.

**Procedure:** Prepare, in triplicate, standard solutions at six concentrations, typically 25, 50, 75, 100, 150, and 200% of target concentration.

**Analysis and acceptance:** Prepare a [calibration curve](calibration.md#calibration-curve) by plotting standard concentration (x-axis) against standard mean response (y-axis). Calculate the [linear regression](data-analysis.md#linear-regression) equation and [coefficient of determination](data-analysis.md#coefficient-of-determination) ($$R^2$$). Accept if$$R^2\geq0.999$$and y-intercept $$\leq2\%$$ of target concentration.

### Precision - Repeatability

**Definition:** The closeness of agreement of multiple measurements of the same sample.

**Procedure:** Prepare one sample containing the target concentration and analyse ten times.

**Analysis and acceptance:** Calculate the mean, standard deviation, and RSD of assay relevant parameters for each sample, e.g. for chromatography, relevant parameters are retention time, peak area, and peak height. Accept if the RSD for each parameter is in the acceptable range, $$\pm5\%$$ for non-regulated products,  $$\pm2\%$$ for dosage forms, and  $$\pm1\%$$ for drug substance.

**Also see:** [Intermediate precision](validation.md#intermediate-precision),  [Reproducibility](validation.md#reproducibility)

### Reproducibility

**Definition:** The [precision ](validation.md#precision)obtained in different labs.

**Procedure:** The same analysis will be performed in two labs. Analysis will be performed on standard solutions at three concentrations, typically 50, 100, and 150% of target concentration.

**Analysis and acceptance:** Calculate the mean, standard deviation, and RSD for labs. Accept if RSD$$\leq2\%$$.

### Robustness

**Definition:** Stability of a method against variations in intrinsic parameters, e.g. for chromatography, mobile phase composition, flow rate, injection volume, and column temperature.

**Procedure:** Analyse the same sample with modified methods. e.g. for chromatography, method modifications will include: mobile phase organic content$$\pm2\%$$; mobile phase pH$$\pm0.1\ pH\ units$$; column temperature$$\pm5\degree C$$.

**Analysis and acceptance:** Changes to intrinsic parameters should not cause a validated method to become invalid by other acceptance criteria.

### Ruggedness

**Definition:** Stability of a method against variations in extrinsic parameters, e.g. analyst, lab, instrument, and day of analysis.

**Procedure:** The same method will be conducted, varying extrinsic parameters.

**Analysis and acceptance:** Changes to extrinsic parameters should not cause a validated method to become invalid by other acceptance criteria.

### Selectivity or Specificity

**Definition:** The extent to which other substances interfere with determination of an analyte.

**Procedure:** Analyse samples spiked with compounds that may be expected to be present in the sample, e.g. excipients.

**Analysis and acceptance:** Determine the [matrix effect](calibration.md#matrix-effect). Accept if $$ME=100\pm15\%$$.

### Stability indicating

**Definition:** Determination of the conditions, if any, under which a given analyte will degrade.

**Procedure:** Store samples in stress conditions. Storage conditions will include:

* $$0.1 M HCl$$,$$0.1 M NaOH$$, intermediate pH values, each at $$40, 60\degree C$$
* $$3\%\ H_2O_2$$at $$25, 60\degree C$$
* Temperature and humidity combinations of $$60, 80\degree C$$ and$$\pm75\% RH$$
* Each condition will be accompanied by a blank control, and tested at$$1,3,5\ days$$.

**Analysis and acceptance:** Determine analyte concentration remaining as$$ST\%=100\left(\frac{[after\ storage]}{[before\ storage]}\right)$$.
