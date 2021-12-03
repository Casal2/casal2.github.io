---
#layout: home
title: Casal2 Release Notes
permalink: /release_notes/
---

# Casal2 Release Notes

## Version 21.11, released 2021-12-03

Craig Marsh, Scott Rasmussen, and Alistair Dunn have made extensive changes, additions, and improvements over the past few months. More information about these changes will be included soon.

This release also updates the MPD reports for the Casal2 [Test Cases](https://github.com/NIWAFisheriesModelling/CASAL2/tree/proportions_at_weight_202101/TestCases/primary). The Test Cases are 6 sets of age-based stock assessment models (labeled `BCO`, `HAK`, `HOK`, `LIN`, `ORH`, and `SBW`) that were constructed to include a [commonly used subset](https://github.com/NIWAFisheriesModelling/CASAL2/raw/master/Documentation/Test_cases_and_functional_requirements_for_Casal2_v1.0.pdf) of the existing functionality. The functionality for the MCMC mode and the projection mode is being validated with the Test Cases.

The Windows installation package for CASAL and the executables for Windows and Linux are in the [TestCases/CASAL subdirectory](https://github.com/NIWAFisheriesModelling/CASAL2/tree/proportions_at_weight_202101/TestCases/CASAL).

### Known issues

The documentation in this release is not complete.

The simulation functionality has not been reviewed or tested.

The CASAL and Casal2 R packages have been tested with R versions 3.6.X only.




## Version 1.1.0, released 2021-07-21

This release is from the [proportions_at_weight_202101](https://github.com/NIWAFisheriesModelling/CASAL2/tree/proportions_at_weight_202101) branch. This is an interim release, as the new observation class was used in the 2021 bluenose (BNS) stock assessment which used Casal2 and followed from [this document](https://fs.fish.govt.nz/Doc/24830/FAR-2020-34-Stock-Assessment-Development-For-Bluenose-4070.pdf.ashx).

This release contains a new observation class, [ProcessRemovalsByWeight](https://github.com/NIWAFisheriesModelling/CASAL2/blob/proportions_at_weight_202101/CASAL2/source/Observations/Age/ProcessRemovalsByWeight.cpp). The [technical specification](https://github.com/NIWAFisheriesModelling/CASAL2/raw/proportions_at_weight_202101/Documentation/Enhancements/Technical_Spec_for_weight_composition.pdf) for this new observation class is in the Documentation/Enhancements subdirectory. The unit test and the R code that produced the values in the unit test are also in the repository.

Casal2 now outputs the covariance matrix from CppAD minimisation.

This release also updates the MPD reports for the Casal2 [Test Cases](https://github.com/NIWAFisheriesModelling/CASAL2/tree/proportions_at_weight_202101/TestCases/primary). The Test Cases are 6 sets of age-based stock assessment models (labeled `BCO`, `HAK`, `HOK`, `LIN`, `ORH`, and `SBW`) that were constructed to include a [commonly used subset](https://github.com/NIWAFisheriesModelling/CASAL2/raw/master/Documentation/Test_cases_and_functional_requirements_for_Casal2_v1.0.pdf) of the existing functionality.

The Windows installation package for CASAL and the executables for Windows and Linux are in the [TestCases/CASAL subdirectory](https://github.com/NIWAFisheriesModelling/CASAL2/tree/proportions_at_weight_202101/TestCases/CASAL).

### Known issues

The executables in this release have known efficiency issues.

The documentation in this release is not complete.

The simulation functionality has not been reviewed or tested.

The CASAL and Casal2 R packages have been tested with R versions 3.6.X only.



## Version 1.0.0, released 2020-08-07

This release tests and validates the functionality used in the Casal2 [Test Cases](https://github.com/NIWAFisheriesModelling/Casal2/tree/master/TestCases/primary). The Test Cases are 6 sets of age-based stock assessment models (labeled `BCO`, `HAK`, `HOK`, `LIN`, `ORH`, and `SBW`) that were constructed to include a [commonly used subset](https://github.com/NIWAFisheriesModelling/CASAL2/blob/master/Documentation/Test_cases_and_functional_requirements_for_Casal2_v1.0.pdf) of the existing functionality.

All of the Test Case Casal2 models were compared with their CASAL counterparts for MPD and MCMC results. The reports of the MPD and MCMC results are in the repository. The projection functionality has been reviewed and tested.

### Known issues

The executables in this release have known efficiency issues and require a review with respect to code optimisation and memory usage. The focus for this release was on testing and validating functionality.

The documentation in this release is not complete.

The simulation functionality has not been reviewed or tested.

Casal2 does not output the covariance matrix from CppAD minimisation.

The CASAL and Casal2 R packages have been tested with R versions 3.6.X only.

