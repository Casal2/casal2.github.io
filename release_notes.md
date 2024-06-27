---
#layout: home
title: Casal2 Release Notes
permalink: /release_notes/
---

# Casal2 Release Notes

The latest version of Casal2 can be downloaded from Github [here](https://github.com/Casal2/CASAL2/releases).

## CASAL2 version 2024.06

CASAL2 received a bunch of code cleanup, minor fixes and updates.
- Added sqrt transformations to manual
- Added mortality constant exploitation process
- Implemented double tag loss
- Added disease mortaloty as an age model process
- Added constant difference parameter transformation
- The user manual has been updated for both Age and Length variants.
- A large number of basic code improvements, error handling and user messages have been updated.
- Building Casal2 and associated documentation has been fixed.
- GitHub Actions have been fixed.
- A new writing your first model tutorial is now available at: https://casal2.readthedocs.io/en/latest/
- Contributor guides, github.io pages etc have all been updated.
- README has been updated.
- Broken unit tests and builds on various Linux platforms and compilers have been fixed.
- Casal2 now supports multiple input configuration files with the -c command like argument

## Version 22.08, released 2022-08-31

Craig Marsh has made extensive changes, additions, and efficiency improvements over the past few months. The main user-facing changes include length-based model functionality, changes to how year class strength (YCS) is defined and used, the generation of simulated observations, additional initialisation types, and the addition of a hybrid fishing mortality process similar to that in [Stock Synthesis 3](https://vlab.noaa.gov/web/stock-synthesis). There is a new length-based Test Case, `SCI`.

There is a new R package in development for post-processing of Casal2 model input and output, [r4Casal2](https://github.com/NIWAFisheriesModelling/r4Casal2).

This release also updates the MPD reports for 7 Casal2 [Test Cases](https://github.com/NIWAFisheriesModelling/Casal2-supporting-information/tree/main/TestCases/primary). The Test Cases are now located in a separate repository. The Test Cases are 6 sets of age-based stock assessment models (labeled `BCO`, `HAK`, `HOK`, `LIN`, `ORH`, and `SBW`) and one length-based stock assessment model (labeled `SCI`) that were constructed to validate a [commonly used subset](https://github.com/NIWAFisheriesModelling/CASAL2/raw/master/Documentation/Test_cases_and_functional_requirements_for_Casal2_v1.0.pdf) of the existing functionality. The functionality for the MCMC mode and the projection mode is being validated with the Test Cases.

### Known issues

The User Manuals and other documentation are not complete.

## Version 21.11, released 2021-12-03

Craig Marsh, Scott Rasmussen, and Alistair Dunn have made extensive changes, additions, and efficiency improvements over the past few months. The main user-facing changes are that tag-release by length and tag-recapture by length have been reviewed and tested, as has time-varying growth.

This release also updates the MPD reports for the Casal2 [Test Cases](https://github.com/NIWAFisheriesModelling/CASAL2/tree/master/TestCases/primary). The Test Cases are 6 sets of age-based stock assessment models (labeled `BCO`, `HAK`, `HOK`, `LIN`, `ORH`, and `SBW`) that were constructed to validate a [commonly used subset](https://github.com/NIWAFisheriesModelling/CASAL2/raw/master/Documentation/Test_cases_and_functional_requirements_for_Casal2_v1.0.pdf) of the existing functionality. The functionality for the MCMC mode and the projection mode is being validated with the Test Cases.

The simulation functionality has been reviewed and tested.

The Windows installation package for CASAL and the executables for Windows and Linux are in the [TestCases/CASAL subdirectory](https://github.com/NIWAFisheriesModelling/CASAL2/tree/master/TestCases/CASAL).

### Known issues

The documentation in this release is not complete.




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

