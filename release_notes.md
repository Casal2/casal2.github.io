---
#layout: home
title: Casal2 Release Notes
permalink: /release_notes/
---

# Casal2 Release Notes

## Version 1.0.0, released 2020-MM-YY

This release tests and validates the functionality used in the Casal2 [Test Cases](https://github.com/NIWAFisheriesModelling/Casal2/tree/master/TestCases/primary). The Test Cases are 6 sets of age-based stock assessment models (labeled `BCO`, `HAK`, `HOK`, `LIN`, `ORH`, and `SBW`) that were constructed to include a commonly used subset of the existing functionality.

All of the Test Case Casal2 models were compared with their CASAL counterparts for MPD and MCMC results. The reports of the MPD and MCMC results are in the repository.

### Known issues

The executables in this release have known efficiency issues and require a review with respect to code optimisation and memory usage. The focus for this release was on testing and validating functionality.

The documentation in this release is not complete.

Casal2 does not output the covariance matrix from CppAD minimisation.

