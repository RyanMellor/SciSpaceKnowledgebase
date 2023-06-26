# Partition and Distribution Coefficients

In pharmaceutical sciences, the partition (logP) and distribution (logD) coefficient are ways of describing [hydrophilicity/hydrophobicity](../../basic-concepts/solvation/#polarity) of a compound ([Comer and Tam, 2007](../../../sources/references.md#comer-j-tam-k-2007-lipophilicity-profiles-theory-and-measurement-in-pharmacokinetic-optimization-in-drug-research-john-wiley-and-sons-ltd-pp-275-304-https-doi-org-10-1002-9783906390437-ch17)).

Partition coefficient are useful as they provide an estimation of a compound’s behaviour in the body. [**ADME** ](../biological-characterization/adme-t.md)describes the **A**bsorption, **D**istribution, **M**etabolization and **E**limination of a compound. The polarity of a compound determines how easily drugs are absorbed and where they will distribute to. Hydrophilic drugs will be found in aqueous compartments such as the blood serum, whereas hydrophobic compounds are more readily distributed to hydrophobic areas such as the lipid bilayers of cells. The partition coefficient also indicates how long a compound will remain in the body and therefore affects its pharmacokinetics. A hydrophobic compound can accumulate in lipophilic tissue and form a reservoir from where the compound is release back into the circulation.

To determine the partition/distribution coefficient, the compound is solubilized in a mixture of two immiscible solvents. At equilibrium the concentration of the compound in each solvent is [determined](../../basic-concepts/concentration.md#methods-of-determination). The ratio of concentrations refers to the partition/distribution coefficient ([Comer and Tam, 2007](../../../sources/references.md#comer-j-tam-k-2007-lipophilicity-profiles-theory-and-measurement-in-pharmacokinetic-optimization-in-drug-research-john-wiley-and-sons-ltd-pp-275-304-https-doi-org-10-1002-9783906390437-ch17)).

$$P=\frac{[solute]_{organic}}{[solute]_{aqueous}}$$

Most commonly, the solvents used are water - which dissolves hydrophilic compounds - and 1-octanol which will dissolve hydrophobic compounds.

**Partition coefficient (LogP):** partition coefficient of a neutral/unionized compound.

$$logP=log\left(\frac{[solute]_{octanol}}{[solute]_{water}}\right)$$

**Distribution coefficient (LogD):** describes the partition of a compound at a specific pH (aqueous phase) and considers the ionized form of the molecule.

$$logD_{pH}=log\left(\frac{[solute]_{octanol}}{[solute]_{water}}\right)$$

The distribution coefficient is informative if the compound is ionized at physiological pH (7.4) ([Clarke and Cahoon, 1987](../../../sources/references.md#clarke-f-h-cahoon-n-m-1987-ionization-constants-by-curve-fitting-determination-of-partition-and-distribution-coefficients-of-acids-and-bases-and-their-ions-journal-of-pharmaceutical-sciences-76-611-620-https-doi-org-10-1002-jps-2600760806)).

## Methods of determination

### Shake-flask

#### Buffer choice

**logP:** The logP of a compound is determined at a pH where the compound is [unionized](pka.md#pka). For a compound with an acidic function this means working at$$pH \leq pKa-2$$ similarly for a base one would work at$$pH \geq pKa +2$$.&#x20;

**logD:** In pharmaceutical sciences, we are interested in how the compound behaves at physiological conditions. Therefore, a good choice of buffer is [potassium phosphate buffer](../../basic-concepts/buffers.md#potassium-phospate) at pH 7.4. However, logD can be determined over the whole range of pH - using appropriate buffers - which provides a distribution profile.

#### **Preparation of solvent mixture**

When preparing the solvents, each solvent has to be saturated by the other. This means some octanol will be mixed into the buffer and buffer will be added to octanol. (This can be obtained with a decantation flask).

The result will be more precise if the amount of drug in both phases is similar ([Andrés et al., 2015](../../../sources/references.md#andres-a-roses-m-rafols-c-bosch-e-espinosa-s-segarra-v-huerta-j-m-2015-setup-and-validation-of-shake-flask-procedures-for-the-determination-of-partition-coefficients-logd-from-low-drug-amounts-european-journal-of-pharmaceutical-sciences-76-181-191-https-doi-org-10-1016-j-ejps-2015-05-008)). If a theoretical/calculated logP/logD is available, the required volume to obtain equal partition, can be calculated for each solvent:

1. $$logP = log\left(\frac{V_{aq}}{V_{org}}\right)$$
2. Let$$log P = 1.17$$
3. $$1.17 = log\left(\frac{V_{aq}}{V_{org}}\right)$$
4. $$10^{1.17} = \frac{V_{aq}}{V_{org}}$$
5. $$14.79 = \frac{V_{aq}}{V_{org}}$$
6. $$V_{aq} = 14.79V_{org}$$
7. Let total volume be 10 mL,$$V_{aq} + V_{org} = 10$$
8. $$V_{org} = 10-V_{aq}$$
9. From equation 6,$$V_{aq}=14.79(10-V_{aq})$$
10. $$V_{aq}=147.9-14.79V_{aq}$$
11. $$15.79*V_{aq}=147.9$$&#x20;
12. $$V_{aq} = 9.37$$mL
13. $$V_{org} = 10 – 9.37 = 0.63$$mL

**Determination of logP and logD**

Prepare a concentration of the compound such that before and after partition the concentration in the aqueous compartment will still be within the calibration curve. As volumes are adjusted to have \~50% of the drug in the organic solvent and 50% of the buffer, a concentration at the higher end of the calibration curve will be chosen.

Prepare the compound at the chosen concentration in the saturated buffer and measure its concentration. Add the required volume of the saturated octanol to the tube and keep it shaking for 24 h. After 24h [determine the concentration](../../basic-concepts/concentration.md#methods-of-determination) in each phase.
