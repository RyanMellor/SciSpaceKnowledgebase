# HPLC - Standard Operating Procedure

{% hint style="info" %}
SOPs will vary greatly with each application, given here is a general outline and best practices.
{% endhint %}

### Mobile Phase and Sample Preparation

* Mobile phase must be compatible with all components of the instruments as well as the column, see manufactures documentation
* If prepared from solid, mobile phase should be filtered to $$0.2\  \mu m$$
* Standard concentration is dependent on column and detector, should be $$<1\ mg/mL$$
* Sample should be fully solubilized, preferably in mobile phase
* Sample can be filtered if necessary however this may affect analyte concentration

### Instrument Preparation

* Ensure waste contained is not full
* Ensure there is a sufficient volume of each solvent and that solvents are connected to the correct lines
* Load column, checking directionality
* Open purge valve and turn on pumps to purge solvent lines of previous solvent and air bubbles
* Turn off pump, close purge valve, and turn the pumps back on
* Check the whole system for leaks
* Equilibrate the system (pressure, temperature, detector) with the number of column volumes recommended by the manufacturer
* Always monitor pressure, a drop may indicate a leak, an increase may indicate a blockage
* Load samples and run acquisition

### Acquisition

#### Method

A method holds the acquisition parameters, specifics will depend on the manufacturer and choice of detector.&#x20;

* **Flow rate:** The flow rate of mobile phase through the system (mL/min)
* **Stop time:** Length of method
* **Post time:** Time between runs, can be used for re-equilibration of the system
* **Solvents:** Initial solvent composition
* **Pressure limits:** Determined by the column, see manufactures documentation. Important to extend the lifetime of the column
* **Timetable:** Allows method parameters to change through the run, e.g. solvent composition, or flow rate. End conditions should match initial conditions to ensure the system is equilibrated for the next run
* **Needle wash:** Minimizes carry over between runs
* **Injection volume:** The amount of sample injected per run
* **Column temperature:** The temperature of the column oven

#### Single sample

Allows injection of one sample at a time, useful for method development to quickly see the effect of changing one method parameter.

#### Sequence

Allows multiple samples, or runs of the same sample, to be injected automatically. User can specify:

* Order of samples/standards/blanks
* Method used for acquisition of each run
* Injection volume (if different to the method)
* Injections per sample

### Analysis

Analysis will depend on the intended application.

* [**Calibration curve**](../../../basic-concepts/calibration.md#calibration-curve)**:** Inject standards of known concentrations, and plot the concentration (x-axis) against area under the curve (AUC, y-axis)
* **Quantification:** Inject sample and compare the AUC a calibration curve
* [**System suitability**](../system-suitability.md#parameters-for-acceptance)**:** Extract the relevant parameters and check against acceptance criteria

