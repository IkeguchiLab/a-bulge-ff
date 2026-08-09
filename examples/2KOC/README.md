# 2KOC Example

This directory contains the system-specific PLUMED implementation of
gHBfix-18Ab for the prepared cUUCGg tetraloop system derived from
PDB ID 2KOC.

## Files

- `scalingParameters.dat`: gHBfix-18Ab correction parameters.
- `typesTable.dat`: gHBfix atom-type assignments for the RNA atoms.
- `plumed.dat`: PLUMED input defining the donor–acceptor atom pairs and
  applying the GHBFIX correction.
- `step3_input.pdb`: prepared structure defining the atom numbering used
  by `typesTable.dat` and `plumed.dat`.

## Important

`typesTable.dat` and the atom indices in `plumed.dat` depend on the exact
atom ordering of `step3_input.pdb`. These files are therefore specific to
the supplied 2KOC-derived system and should not be directly applied to a
different structure or atom ordering.

The `scalingParameters.dat` file contains the same final gHBfix-18Ab
parameter set provided in `../../parameters/`.
