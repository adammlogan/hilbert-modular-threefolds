Readme file for code to accompany the paper "Kodaira dimension of Hilbert
modular threefolds"

This code consists of files to compute defects, both individually and
asymptotically, and to reconstruct the examples and tables in sections
6 and 7 of the paper.  There are no special installation instructions;
simply extract the files into a single directory.  All of the functions
may be loaded by loading the file "loadall.mag".

These functions depend on some functions from the Hilbert modular forms
package at https://github.com/edgarcosta/hilbertmodularforms/.  You may
need to change lines reading

AttachSpec("~/magmalib/hilbertmodularforms/spec");

to refer to the correct path on your system.

We briefly describe the individual files in the package.  Each file begins
with a brief listing of functions intended for users.

algorithms.mag      Functions that implement each of the numbered algorithms in the paper.
cq-defect.mag       Functions to calculate defects of cyclic quotient singularities.
defect-new.mag      A function to compute individual defects of cusps.
dimension.mag       A function to evaluate the Thomas-Vasquez formula for the Hilbert series of the ring of level 1 forms.
ex61-63.mag         Code to reproduce examples 6.1 and 6.3 in the paper.
ex67.mag            Code to reproduce example 6.7 in the paper.
fields.mag          List of cubic fields (from the LMFDB).
grundman-chi.mag    A function that evaluates the genus of a Hilbert modular threefold for level 1.
loadall.mag         Load all the files, except ex*.mag and maybe-gen-type.mag which are scripts rather than collections of functions, and the long list of cubic fields.
lucant-dim.mag      Evaluate the dimension formula given in section 5.1 of \cite{hmf-mult}.
manycubics.mag      Long list of cubic fields, downloaded from the LMFDB.
maybe-gen-type.mag  Script to look for additional fields for which the Hilbert modular threefold may not be of general type.
minimal.mag         Functions to determine the trace-minimal cone and the set of reducers.
polyhedra.mag       Functions to set up the union of polyhedra and calculate its volume.
qz.mag              Define Q, Z to be the rationals and integers respectively.
tables-sec6.mag     Recompute the tables in section 6.
tables-sec7.mag     Recompute the tables in section 7.

All computations were done using Magma 2.28-3 on the author's laptop, a
machine with 16 gigabytes of memory and an Intel i7-11390H processor
with 8 cores running at 3.40 GHz.
