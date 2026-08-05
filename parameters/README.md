# gHBfix-18Ab Parameter Files

This directory contains the final gHBfix-18Ab hydrogen-bond correction
parameter definition.

gHBfix-18Ab consists of 18 correction terms defined by three donor
categories (NH, NH2, and 2'-OH) and six acceptor categories
(N, O, O4', 2'-OH, bO, and nbO).

## Files

| File | Description |
|---|---|
| `scalingParameters.dat` | Parameter file in the format read by the PLUMED `GHBFIX` action |
| `parameter_matrix.tsv` | Human-readable 3 × 6 matrix of the final 18 correction terms |
| `atom_type_mapping.tsv` | Mapping between numerical implementation identifiers and donor/acceptor categories |

## Relationship between the files

`scalingParameters.dat` is the machine-readable parameter file used by
PLUMED.

`parameter_matrix.tsv` presents the same scientific parameter definition
as a donor-by-acceptor matrix for easier inspection and comparison with
the associated article.

`atom_type_mapping.tsv` explains the numerical type identifiers used in
`scalingParameters.dat` and in system-specific atom-type assignment files.

## Atom-type identifiers

The numerical type identifiers are implementation labels and are not
physical quantities.

Type identifiers 1–8 were retained from the original gHBfix input
convention. Type 17 was introduced in this study to distinguish NH2 donor
hydrogens from the original NH donor category. The numerical value 17 is
arbitrary and has no physical meaning.

## Correction strengths

Correction strengths are reported as kBTλ in kcal mol−1, following the
convention used in the associated article.

Positive values favor the corresponding interaction, whereas negative
values disfavor it. Terms assigned a value of 0.0 are retained explicitly
because they are part of the final gHBfix-18Ab parameter definition.

## Scope

The files in this directory define only the gHBfix-18Ab hydrogen-bond
correction parameters.

They do not include:

- atom-type assignments for a particular RNA structure;
- donor–acceptor atom-pair lists;
- GROMACS topology or MD input files;
- OL3CP parameters;
- NBfix0BPh parameters; or
- other force fields evaluated in the associated study.

A system-specific implementation example for the prepared 6VA1-derived
system is provided under [`../examples/6VA1/`](../examples/6VA1/).

## Citation

Please cite the associated article and the original gHBfix methodology
when using these parameters.
