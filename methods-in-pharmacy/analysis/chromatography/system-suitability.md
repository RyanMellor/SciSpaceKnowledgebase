# System Suitability

Definitions are from USP <621> ([USP General, 2012](../../../sources/references.md#usp-general-2012-less-than-621-greater-than-chromatography-united-states-pharmacopeia-40-508-520))

## Factors Affecting System Suitability

* [Mobile phase](high-performance-liquid-chromatography/method-development.md#mobile-phase-eluent) - Composition, ionic strength, temperature, and pH
* [Column ](high-performance-liquid-chromatography/method-development.md#stationary-phase-column)- dimensions, particle size, pore size, chemistry of stationary phase
* [Instrument settings](high-performance-liquid-chromatography/method-development.md#instrument-settings) - Flow rate, injection volume, column temperature, data collection rate

## Parameters for Acceptance

### Efficiency - Number of Theoretical Plates ($$N$$)

A measure of column efficiency, used to compare performance of different columns. More efficient columns have higher$$N$$, i.e. sharper peaks at a given$$t_R$$.

$$N = 16\left(\frac{t_R}{W}\right)^2$$ or $$N=5.54\left(\frac{t_R}{W_\frac{h}{2}}\right)^2$$

Where:

* $$t_R$$= [Retention time](system-suitability.md#retention-time)
* $$W$$= Baseline width of the peak
* $$W_\frac{h}{2}$$ = Half height width of the peak

**Acceptance criteria:** $$N>2000$$

![Baseline width and half height width](<../../../.gitbook/assets/image (81).png>)

### Injection Reproducibility

[RSD ](../../basic-concepts/data-analysis.md#relative-standard-deviation)for peak area, height, and retention time.

**See:** [Precision](../../basic-concepts/validation.md#precision-repeatability)

**Acceptance criteria:** $$\%RSD \leq1,\ for\ n\geq6$$

### Resolution ($$R_S$$)

The separation of two compounds.

$$R_S=\frac{2(t_{R2}-t_{R1})}{W_1+W_2}$$ or $$R_S=\frac{1.18(t_{R2}-t_{R1})}{W_{1,\frac{h}{2}}+W_{2,\frac{h}{2}}}$$

Where:

* $$t_{R2}$$= [Retention time](system-suitability.md#retention-time) of analyte
* $$t_{R1}$$= [Retention time](system-suitability.md#retention-time) of reference compound
* $$W_1$$ = Baseline width of peak 1
* $$W_2$$ = Baseline width of peak 2
* ​​$$W_{1,\frac{h}{2}}$$​​ = Half height width of peak 1
* $$W_{2,\frac{h}{2}}$$​​ = Half height width of peak 2

Alternatively defined by the **Purnell equation** (assuming equal peak width):

$$R_S=\frac{\sqrt{N_2}}{4} \frac{k_2}{1+k_2} \frac{\alpha-1}{\alpha}$$

Where:

* $$N_2$$= [Efficiency ](system-suitability.md#efficiency-number-of-theoretical-plates)of the second peak
* $$k_2$$= [Retention factor](system-suitability.md#retention-or-capacity-factor) of the second peak
* $$\alpha$$= [Separation factor](system-suitability.md#separation-factor) of the two peaks

This form highlights the effect of various parameters on resolution. Where, increasing $$k$$ or $$N$$ has dismissing returns after a certain point, and increasing $$\alpha$$ has the greatest impact on resolution.

**Acceptance criteria:** $$R_S>2$$

![](<../../../.gitbook/assets/image (16).png>)

### Retention or Capacity Factor ($$k$$)

The retention time of a peak relative to the hold-up time.

$$k=\frac{t_R-t_M}{t_M}$$

Where:

* $$t_R$$ = [Retention time](system-suitability.md#retention-time)
* $$t_M$$ = [Hold-up time](system-suitability.md#hold-up-time)

**Acceptance criteria:** $$k>2$$

### Symmetry or Tailing Factor ($$S,T$$)

$$S,T=\frac{W_{0.05}}{2f}$$

Where:

* $$W_{0.05}$$ = 5 % height width of the peak
* $$f$$ = 5 % height distance from peak maximum to leading edge

**Acceptance criteria:** $$S,T\leq2$$

![](<../../../.gitbook/assets/image (42).png>)

## Other Parameters

### Dwell Time and Volume ($$t_D,V_D$$)

The volume between the point at which the eluents meet and the top of the column. Must be considered during gradient elution, a change at the gradient valve will take some time to affect conditions on the column.

**Determination**

* Method
  * Mobile phase:
    * (A) $$H_2O$$
    * (B) $$H_2O$$, 0.2% Acetone
  * Flow rate ($$F$$): 1 mL/min
  * Gradient: 0-100 %B 10 mins
  * Column: None, stainless steel connector
  * Detection: 265 nm
*   Analysis

    * Plot straight line through original baseline
    * Plot straight line through gradient portion of response
    * $$t_D$$is the intercept of these two lines
    * $$V_D = t_D F$$



![](<../../../.gitbook/assets/image (13).png>)

![](<../../../.gitbook/assets/equipment - HPLC - dwell volume.png>)

### Height Equivalent to a Theoretical Plate ($$H, HETP$$)

A measure of column efficiency

* Pathways within the column ($$A$$, independent of $$\mu$$)
* Axial and longitudinal diffusion ($$\frac{B}{\mu}$$, negligible for practical values of $$\mu$$)
* Mass transfer kinetics between stationary and mobile phases ($$C\mu$$, increases linearly with $$\mu$$).

Defined by the **van Deemter equation**:

$$H = \frac{L}{N}=A+\frac{B}{\mu}+C\mu$$

Where:

* $$L$$ = Column length
* $$N$$ = [Efficiency](system-suitability.md#efficiency-number-of-theoretical-plates)
* $$A$$ = Eddy-diffusion parameter
* $$B$$ = Diffusion coefficient
* $$C$$ = Resistance to mass transfer coefficient
* $$\mu$$ = Linear velocity

$$A = 2\lambda d_p$$

$$B=2\gamma D_M$$

$$C = C_s+C_m=\frac{f_s(k){d_p}^2}{D_s}+\frac{f_m(k){d_f}^2}{D_m}$$

Where:

* $$\lambda$$ and $$\gamma$$ = Stationary phase packing constants
* $$d_p$$ = Particle diameter
* $$d_f$$ = Thickness of liquid film on stationary phase
* $$D_S$$ and $$D_M$$ = Stationary and mobile phase diffusion coefficients
* $$C_s$$ and $$C_m$$ = Stationary and mobile phase broadening
* $$f_s(k)$$ and $$f_m(k)$$ = Functions of capacity factor, partition ratios between stationary and mobile phase

![](<../../../.gitbook/assets/image (5).png>)

### Hold-Up Time ($$t_M, t_0$$)

The time required for elution of an unretained compound. The symbol $$t_0$$is often used.

![Hold-up time and retention time](<../../../.gitbook/assets/image (75).png>)

### Hold-Up Volume ($$V_M$$)

The volume of mobile phase required for elution of an unretained compound. In size exclusion chromatography, the symbol $$V_0$$ is used.

$$V_M = t_M F$$

Where:

* $$t_M$$ = [Hold-up time](system-suitability.md#hold-up-time)
* $$F$$ = Flow rate of mobile phase

### Linear Velocity ($$\mu$$)

The speed at which mobile phase is moving.

$$\mu = \frac{L}{t_M}$$

Where:

* $$L$$ = Column length
* $$t_M$$ = Hold-up time

Linear velocity allows for comparison of mobile phase speed for columns with differing diameters. Is unchanged by any system variables for a given column and flow rate.

### Peak-to-Valley Ratio ($$p/v$$)

Employed when peak separation is not achieved. Ratio of the height of the peak to the height of the valley between two peaks.

$$p/v = \frac{H_p}{Hv}$$

Where:

* $$H_p$$ = Height of peak
* $$H_v$$ = Height of valley

![Height of peak and height of valley](<../../../.gitbook/assets/image (65).png>)

### Relative Retardation ($$R_{ret}$$)

Used in planar chromatography. The ratio of the distance travelled by an analyte and a reference compound.

### Relative Retention($$r$$)

The ratio of the retention time of an analyte and a reference compound.

$$r=\frac{t_{R2}-t_M}{t_{R1}-t_M}$$

Where:

* $$t_{R2}$$= [Retention time](system-suitability.md#retention-time) of analyte
* $$t_{R1}$$= [Retention time](system-suitability.md#retention-time) of reference compound
* $$t_M$$ = [Hold-up time](system-suitability.md#hold-up-time)

### Retardation Factor ($$R_F$$)

Used in planar chromatography. The ratio of the distance travelled by an analyte and the mobile phase.

### Retention Time ($$t_R$$)

The time between injection and a peak maximum.

### Retention Volume($$V_R$$)

The volume of mobile phase required for elution of a compound.

$$V_R=t_RF$$

Where:

* $$t_R$$ = [Retention time](system-suitability.md#retention-time)
* $$F$$ = Flow rate of mobile phase

### Separation Factor ($$\alpha$$)

The ratio of capacity factors of two adjacent peaks.

$$\alpha=\frac{k_2}{k_1}$$

Where:

* $$k_2$$ = [Capacity factor](system-suitability.md#retention-or-capacity-factor) of peak 2
* $$k_1$$ = [Capacity factor](system-suitability.md#retention-or-capacity-factor) of peak 1

### Signal-to-Noise Ratio ($$S/N$$)

Measured over a distance of $$\geq5$$ times the half height width of peak.

$$S/N = \frac{2H}{h}$$

Where:

* $$H$$ = Height of peak from maximum to extrapolated baseline
* $$h$$ = Difference between smallest and largest noise values

![Signal-to-noise ratio](<../../../.gitbook/assets/image (53).png>)
