# anion-and-osmolar-gap
web calculator for anion gap and osmolar gap

![](https://github.com/nickmmark/anion-and-osmolar-gap/blob/main/osmolar-gap_demo.gif)

try it yourself [here](https://nickmmark.github.io/anion-and-osmolar-gap/)


### Calculations
Anion Gap:
```math
AG = Na - (Cl + HCO_3)
```

Albumin-corrected Anion Gap:
```math
AG_{corr} = AG + 2.5 \times (4.0 - Albumin)
```

Calculated Serum Osmolality (US Units)
```math
Osm_{calc} = 2 \times Na + \frac{Glucose}{18} + \frac{BUN}{2.8} + \frac{Ethanol}{3.7}
```

### Differential Diagnosis
The app automatically displays the differential diagnosis.

High anion gap:
* Glycols (ethylene glycol, propylene glycol)
* Oxoproline (APAP metabolite)
* L-lactate
* D-lactate
* Methanol
* Aspirin (salicylates)
* Renal failure (uremia)
* Ketoacidosis


### Functions
* normalizeInputs() - Converts all user inputs into a consistent internal unit system.
* calcAnionGap() - Computes raw anion gap.
* calcCorrectedAG() - Applies albumin correction.
* calcOsmolality() - Computes calculated serum osmolality.
* calcOsmGap() - Computes osmolar gap.
* calculateAndRender() - Central render loop that updates outputs and flags on input changes.

### References
Glasser L, Sternglanz PD, Combie J, Robinson A. [Serum osmolality and its applicability to drug overdose](https://pubmed.ncbi.nlm.nih.gov/4751712/). Am J Clin Pathol. 1973
