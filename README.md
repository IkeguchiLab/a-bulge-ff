# gHBfix-18Ab Parameters for the RNA A-Bulge Motif

This repository provides the final gHBfix-18Ab hydrogen-bond correction
parameters developed for the RNA A-bulge motif and system-specific PLUMED
implementation examples for the MAPT pre-mRNA A-bulge system derived from
PDB ID 6VA1 and the cUUCGg tetraloop system derived from PDB ID 2KOC.

The 6VA1 example corresponds to the A-bulge system used for development and
evaluation of gHBfix-18Ab, whereas the 2KOC example corresponds to the
tetraloop system used for reference-structure retention testing.

## Scope

This repository is limited to the gHBfix-18Ab correction developed in this
study. It does not provide all force fields and correction schemes evaluated
in the associated article.

The gHBfix parameters used in the gHBfix-18Ab and gHBfix-18Ab* simulations
are identical. The asterisk denotes the additional use of the OL3CP and
NBfix0BPh corrections and does not represent a different gHBfix parameter set.

The repository includes system-specific gHBfix-18Ab implementation examples
for 6VA1 and 2KOC, but does not include the OL3CP or NBfix0BPh components
used in the composite gHBfix-18Ab* model.
