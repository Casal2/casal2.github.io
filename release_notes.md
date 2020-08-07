---
#layout: home
title: Casal2 Release Notes
permalink: /release_notes/
---

# Casal2 Release Notes

## Version 1.0.0, released 2020-08-07

This release tests and validates the functionality used in the Casal2 [Test Cases](https://github.com/NIWAFisheriesModelling/Casal2/tree/master/TestCases/primary). The Test Cases are 6 sets of age-based stock assessment models (labeled `BCO`, `HAK`, `HOK`, `LIN`, `ORH`, and `SBW`) that were constructed to include a [commonly used subset](https://github.com/NIWAFisheriesModelling/CASAL2/blob/master/Documentation/Test_cases_and_functional_requirements_for_Casal2_v1.0.pdf) of the existing functionality.

All of the Test Case Casal2 models were compared with their CASAL counterparts for MPD and MCMC results. The reports of the MPD and MCMC results are in the repository. The projection functionality has been reviewed and tested.

### Known issues

The executables in this release have known efficiency issues and require a review with respect to code optimisation and memory usage. The focus for this release was on testing and validating functionality.

The documentation in this release is not complete.

The simulation functionality has not been reviewed or tested.

Casal2 does not output the covariance matrix from CppAD minimisation.

The CASAL and Casal2 R packages have been tested with R versions 3.6.X only.

