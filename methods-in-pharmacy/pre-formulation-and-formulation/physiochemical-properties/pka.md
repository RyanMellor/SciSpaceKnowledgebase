# pH and pKa

## pH

The **acidity** and **basicity** of an aqueous solution is expressed by it’s pH. An aqueous solution of acids has a pH below 7, an aqueous solution of bases has a pH above 7, and pure water has a pH of 7.

The pH is defined as the negative decimal logarithm of the hydrogen ion activity ($$aH^+$$) in a solution.

$$pH = - log_{10}(aH^+) = log_{10} (\frac{1}{aH^+})$$

The activity coefficient is a function of the ion concentration and approaches 1 as the solution becomes increasingly dilute. Therefore, hydrogen ion concentration and hydrogen ion activity are nearly equal in very dilute samples. For simplicity reasons, the pH is often calculated as:

$$pH = - log_{10}([H^+])$$

pH measurement is inversely proportional to temperature, what is actually changing is the neutral point, for pure water $$[H^+] = [OH^-]$$ independent of temperature.

## pKa

An **acid** is defined as a molecule/ion capable of donating a proton ($$H^+$$), conversely a **base** is defined as a molecule/ion capable of accepting a proton.

Acid: $$HA \rightleftharpoons A^- + H^+$$

Base: $$B + H^+ \rightleftharpoons  BH^+$$

The pKa of an acid or a base defines its strength as it translates to its dissociation constant of a solution. It is defined as the negative decimal logarithm of the acid dissociation constant (Ka) of a solution.

$$pKa = -log_{10}Ka$$

In the case of an acid, the lower it’s pKa value, the stronger the acid is. The opposite is true for a base. The pKa also informs about the proportion of H+ dissociated/associated.

At pH = pKa: 50% of the molecule is ionized.

For an acid at pH = pKa +2 more than 99.9% of the molecule is ionized. For a base the same is true at pH = pKa – 2.

### **Determination of pKa**

#### Titration

**Definition:** The process of adding known volumes of an acid or base at known concentration is called titration.

**Procedure:** A molecule is dissolved in water. An acid compound is titrated using a strong base whereas a basic compound is titrated with a strong acid. The pH value of the solution is monitored during the process.

**Analysis:** The equivalence point is characterized by a pronounced change in pH when adding small volumes of the titrant. The pKa value of the compound corresponds to the pH at half the equivalence volume and can be obtained by taking the first derivative or using the tangent method ([Babić et al., 2007](../../../sources/references.md#babic-s-horvat-a-j-m-mutavdzic-pavlovic-d-kastelan-macan-m-2007-determination-of-pka-values-of-active-pharmaceutical-ingredients-trac-trends-in-analytical-chemistry-26-1043-1061-https-doi-org-10-1016-j-trac-2007-09-004)).

**Pros:** Accurate, precise

**Cons:** Low sensitivity$$\sim10^{-4} M$$, carbonate free solution

#### Spectrophotometric method

**Overview:** pKa may be determined spectrophotometrially if the compound undergoes a colour change (change in absorption spectra) upon a change in ionization state, i.e. is halochromic.

**Procedure:** Absorption spectra are obtained of the compound in its protonated and deprotonated form. The optimum wavelength for pKa determination is the highest wavelength that displays an ionization-dependant absorbance. The spectrum of the compound in solution is measure in a series of buffer solutions with known pH values ([Dubey et al., 2017](../../../sources/references.md#dubey-s-m-singhvi-g-tyagi-a-agarwal-h-krishna-k-v-2017-spectrophotometric-determination-of-pka-and-log-p-of-risperidone-journal-of-applied-pharmaceutical-science-7-155-158)). Ideally, buffers at $$pH = pKa \pm 0, 0.2, 0.4,0.6$$ are prepared, this requires a theoretical/calculated pKa value for the molecule.

**Analysis:** pKa is the mean of the values obtained from the equation below for each sample.

Base: $$pKa = pH + log\left(\frac{|A-A_N|}{|A_I – A|}\right)$$

Where:

* $$A$$ = Absorbance
* $$A_I$$ = Absorbance of ionized compound
* $$A_N$$ = Absorbance of neutral compound

**Cons:** Chromophore, difference spectra of ionized/non-ionized compound

**Pros:** High sensitivity$$\sim10^{-6} M$$, precision
