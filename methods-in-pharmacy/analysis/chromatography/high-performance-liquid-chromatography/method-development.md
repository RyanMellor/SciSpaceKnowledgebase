# HPLC - Method Development

{% hint style="info" %}
It is common practice to have aqueous mobile phase on line A and organic phase on line B, therefore 'B' is used synonymously with 'organic component'
{% endhint %}

![](<../../../../.gitbook/assets/image (63).png>)

## Mobile Phase (eluent)

**General considerations**

* Mobile phase components should be measured out separately before mixing, do not assume that the volume of a mixture is equal to the sum of component volumes
* If the instrument does not contain a degassing unit then the mobile phase should be degassed before use
* If prepared from solid, mobile phase should be filtered to$$0.2\  \mu m$$

**Polarity**

* Primary method of altering analyte retention
* Solvent strength depends on the mode of separation, e.g. non-polar solvent are weak eluents for [normal phase](../methods-of-separation.md#normal-phase) but strong eluents for [reversed phase](../methods-of-separation.md#reversed-phase)

**Buffers and Salts**

* Ensure the selected pH is compatible with the column
* If the analyte is ionizable then retention will usually be affected by pH as ionization state affects polarity
* Most repeatable results will be obtained when $$>90\%$$of the analyte in non-ionized
* The mobile phase pH should be within $$\pm 1$$ pH unit of the buffering ion pKa
* It is common to use a non-buffered but sufficiently low pH mobile phase, e.g. $$0.1\%$$ TFA
* Buffer/salt will limit the highest usable %B, e.g. phosphate buffer will precipitate at $$\sim 70\%$$ACN or $$\sim 80\%$$MeOH
* Buffer/salt selection may be limited by the detection method, e.g. MS and ELSD require volatile mobile phase, and UV-Vis absorbance requires the mobile phase be transparent at the detection wavelength
* For UV-Vis detection, a level baseline can be achieved by having different modifier concentrations in A and B, e.g. $$0.1\%$$ TFA/H2O and $$0.085\%$$ TFA/ACN

## Stationary Phase (column)

**Bonded phase**

* Selected based on the appropriate mode of [separation](../methods-of-separation.md) for the analyte

**Length**

* Shorter columns reduce runtime and back pressure

**Internal Diameter**

* Narrower columns reduce the flow rate required to obtain a given linear velocity, therefore reducing solvent consumption

**Particle Size**

* Smaller particle size allows for more efficient packing and therefore better column efficiency
* Back pressure is inversely proportional to the square of particle diameter, i.e. halving the particle size increases pressure by a factor of 4

**Pore Size**

* Selection is determined by analyte molecular weight
  * **Small molecules:** 60-120 Å
  * **Small molecules and peptides:** 80-150 Å
  * **Polypeptides and proteins:** 200-450 Å
  * **High molecular weight proteins:** 1000-4000 Å

## Instrument settings&#x20;

**Flow rate**

* Higher flow rates reduce runtime by increasing [linear velocity](../system-suitability.md#linear-velocity)
* Higher flow rates increase back pressure
* [HETP](../system-suitability.md#height-equivalent-to-a-theoretical-plate) describes the effect of linear velocity on efficiency

**Injection volume**

* Determined by sample concentration and instrument sensitivity
* Generally better to inject small volumes of concentrated analyte
* Large volumes should only be used if it is not possible to pre-concentrate the sample
* Injecting too much sample will lead to column overload, band broadening, and peak asymmetry

**Column temperature**

* Higher temperatures reduce mobile phase viscosity and therefore back pressure

**Data collection rate**

* Should be set higher for faster eluting (narrow peak) compounds

## Back pressure

$$\Delta P=\frac{\eta FL}{K^0\pi r^2{d_p}^2}$$

Where:

* $$\Delta P$$ = Change in pressure
* $$\eta$$ = Viscosity
* $$F$$ = Flow rate
* $$L$$ = Column length
* $$K^0$$ = Column permeability
* $$r$$ = Column radius
* $$d_p$$ = Particle diameter

Therefore, all else being equal, back pressure is:

* **Directly proportional to:** viscosity, flow rate, and column length
  * Higher temperature will decrease viscosity, reducing back pressure
  * Solvent viscosities vary leading to different back pressure
* **Inversely proportional to:** column permeability
* **Inversely proportional to the square of:** column radius, and particle diameter

## Isocratic Elution

Eluent composition (and therefore strength) remains constant throughout the run.

**Advantages**

* Simplicity
* No need to re-equilibrate column between samples

**Optimization (for reversed phase, vice versa for normal phase)**

* Run method with 100 %B
* Decrease %B in 10% steps until desired retention is achieved
  * A 10% decrease in B results in \~3x increase in k
* Optimize resolution by varying:
  * **pH:** the analyte should be unionized
  * **Organic solvent:** ACN, MeOH, or THF
  * **Column dimensions:** longer narrower columns with smaller particles have higher efficiency but also higher back pressure
  * **Flow rate:** there will be a flow rate where efficiency is optimized, and a change in either direction will be detrimental
  * **Temperature:** higher temperatures can increase efficiency by reducing viscosity and increasing diffusion rates. A $$1\degree C$$ increase will decrease k by $$\sim 1-2 \%$$
  * **Injection volume/sample concentration:** higher volumes/concentrations will increase peak width
* If $$R_s$$ does not meet acceptance criteria, use a different stationary phase and repeat previous steps
* or
* If $$R_s$$ does not meet acceptance criteria, switch to a gradient elution

## Gradient Elution

Eluent composition (and therefore strength) is steadily changed throughout the run.

**Advantages**

* Analytes with very different retentions
* Strongly retained impurities
* Scouting mobile phase composition
* Generally results in narrower and more consistent width peaks

**Optimization (for reversed phase, vice versa for normal phase)**

* Run a gradient method from 5-100 %B (buffer permitting) over 30 minutes
* Hold at 100 %B to ensure all sample components have eluted
* Initial and final composition are determined by the first and last eluted component. Calculate the solvent composition at [$$t_R$$](../system-suitability.md#retention-time)-[$$t_D$$](../system-suitability.md#dwell-time-and-volume)
*   Solvent composition should always return to initial conditions to allow re-equilibration before further injections

    Optimize resolution by varying parameters as with isocratic elution
* If $$R_s$$ does not meet acceptance criteria, consider a stepped gradient

$$k^*=\frac{t_GF}{S\Delta \Phi V_m}$$

Where:

* $$k^*$$ = Gradient capacity factor
* $$t_G$$ = Gradient time
* $$F$$ = Flow rate
* $$S$$ = Constant, based on analyte size
* $$\Delta \Phi$$ = Change in volume fraction of B
* $$V_m$$ = Column void volume

## Effect of Each Variable

See [System Suitability](../system-suitability.md) for an explanation of each variable

![](<../../../../.gitbook/assets/image (27).png>)

![](<../../../../.gitbook/assets/summary - HPLC composite vars.png>)
