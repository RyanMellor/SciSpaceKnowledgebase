# Methods of Separation

![](<../../../.gitbook/assets/process - chromatography.png>)

## Support

The material to which the bonded phase is bonded.

**Silica**

* Most common support
* pH range: 2-8
* Silanol groups (Si-OH) are reacted with a bonding reagent, e.g. octyldimethyl silane leads to C8 bonded phase
* Residual silanols are end-capped, e.g. reacted with trimethyl silane

**Polymer**

* Commonly used for bioseparations and ion exchange
* pH range: 1-14
* commonly cross-linked polystyrene-divinylbenzene, polyethers, and polymethacrylates

**Carbohydrate-based**

* Common for affinity chromatography
* Agarose, cellulose

**Hybrid**

## Partition

### Normal Phase

* **Mobile phase:** Non-polar (hexane, toluene, ethyl acetate)
* **Elution order:** Least polar first
* **Stationary phase:** Polar
  * **Silica (Si):** Separation of polar, non-ionic organics
  * **Amino (NH₂):** Separation of sugars, alcohols, carbohydrates. Also, weak anion exchange
  * **Diol:** Robust alternative to silica. Also, commonly used for size exclusion

![](<../../../.gitbook/assets/process - separation - normal - bonded.png>)

Separation is achieved based on partition of analyte between the non-polar mobile phase and the polar stationary phase. Polar analytes favour interaction with the stationary phase and are retained longer. Non-polar compounds elute first.

![](<../../../.gitbook/assets/separation - normal (1).png>)

### Reversed Phase

* **Mobile phase:** Polar (water + organic modifier)
* **Elution order:** Most polar first
* **Stationary phase:** Non-polar
  * **Cyano (CN):** Different selectivity to Cx, imporoved retention of polar compounds
  * **Amide (C(=O)N):** For polar compounds, e.g. carbohydrates and peptides
  * **Pentafluorophenyl (PFP):** For polar analytes, aromatic and unsaturated compounds, phenols, and halogenated compounds
  * **Butyl (C4):** Less retentive than C18 or C8, preferred for protein separations
  * **Octyl (C8):** Similar to C18 but less retentive, preferred for more polar analytes
  * **Phenyl:** For medium polarity analytes, e.g. proteins, preferred for aromatics
  * **Octadecyl (C18):** Very hydrophobic, most common choice for separations

![](<../../../.gitbook/assets/process - separation - reversed - bonded.png>)

Separation is achieved based on partition of analyte between the polar mobile phase and the non-polar stationary phase. Non-polar analytes favour interaction with the stationary phase and are retained longer. Polar compounds elute first.

![](<../../../.gitbook/assets/separation - reversed (1).png>)

## Size Exclusion

* **Elution order:** Largest analytes first
* **Application:** Macromolecules, synthetic polymers, biomolecules

Separation is achieved based on molecular size of analyte. Smaller analytes can travel in and out of pores in the stationary phase and therefore have a greater path length to traverse. The opposite is true for larger analytes.

**Gel Filtration Chromatography (GFC)** uses an aqueous mobile phase

**Gel Permeation Chromatography (GPC)** uses an organic mobile phase

If the degree of polymerization is distributed, as is often the case with polymers, the molar mass distribution can be defined in a number of ways, each of which relate the number ($$N_i$$) and molar mass ($$M_i$$) of each species in the sample.

**Number average molecular weight (**$$M_n$$**)** is the arithmetic mean of molecular masses for each species in a sample.

$$M_n = \frac{\sum N_iM_i}{\sum N_i}$$

**Weight average molecular weight (**$$M_W$$**)** takes into account the size of each species, larger molecules have a larger impact.

$$M_W = \frac{\sum N_iM_i^2}{\sum N_iM_i}$$

**Molar mass dispersity (**$$Đ_M$$**)** quantifies how disperse a sample is. Also called polydispersity index (PDI).

$$Đ_M=\frac{M_W}{M_n}$$

![](<../../../.gitbook/assets/separation - sec.png>)

## Ion Exchange

* **Mobile phase:** Aqueous, buffer + salt
* **Elution order:** Controlled by changing pH or counter ion concentration
* **Application:** Biomolecule analysis and purification
* **Stationary phase:** Ionic
  * Strong and weak cation exchange (SCX, WCX)
    * **Carboxymethyl (CM):** Weakly acidic
    * **Sulfate (S):** Strongly acidic
  * Strong and weak anion exchange (SAX, WAX)
    * **Diethylaminoethyl (DEAE):** Weakly basic
    * **Polyethyleneimine (PEI):** Weakly basic
    * **Quaternary ammonium (Q):** Strongly basic

![](<../../../.gitbook/assets/process - separation - iex - bonded.png>)

Separation is achieved based on electrostatic interaction between analyte and stationary phase. The column is first equilibrated with an appropriate counter ion (opposite charge to that of the stationary phase). A mixture containing the analyte is then passed over the column and analyte displaces the counter ion. The analyte is eluted either by changing the pH such that the molecule loses its charge, or by increasing the concentration of counter ion.

![](<../../../.gitbook/assets/separation - iex.png>)

## Affinity

* **Mobile phase:** Aqueous, buffer + salt
* **Elution order:** Controlled by changing ligand or salt concentration
* **Application:** Biomolecule purification
* **Stationary phase:** Analyte specific ligand
  * **Antibodies:** Complimentary antigens
  * **Enzyme substrates:** Enzymes
  * **Nucleic acid:** Complimentary sequence
  * **Lectins:** Sugars, polysaccharides
  * **Boronates:** Sugars, polysaccharides
  * **Metal chelates:** Metal binding biomolecules

Separation is achieved based on specific interactions between analyte and target ligand. A ligand for which the analyte has a high affinity is bound to the stationary phase, e.g. antibody/antigen, enzyme/substrate, or nucleic acid/complementary sequence. A mixture containing the analyte is then passed over the column, the analyte binds while other molecules are non retained. The analyte is eluted either by introduction of a soluble ligand, or by increasing the concentration of salt.

![](<../../../.gitbook/assets/separation - affinity.png>)
