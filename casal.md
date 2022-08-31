---
#layout: home
title: CASAL Files for Windows and Linux
permalink: /casal/
---

# CASAL

[CASAL](https://niwa.co.nz/fisheries/tools-resources/casal) is the predecessor of Casal2. It is used for quantitative stock assessments for many of New Zealand's fish stocks, including deepwater (e.g., orange roughy), middle depth (e.g., hoki), inshore (e.g., snapper), and shellfish fisheries. Internationally, it has been used to assess Patagonian and Antarctic toothfish, and broadbill swordfish fisheries.

## CASAL User Support Forums

Please post questions about and issues with CASAL on the [Casal2 Discourse site](https://casal2.discourse.group).

## CASAL files for Windows and Linux

[CASAL User Manual for version 2.30](https://github.com/NIWAFisheriesModelling/Casal2-supporting-information/raw/main/TestCases/CASAL/casalv230-2012-03-21.pdf)

Executable files
- [Windows executable for version 2.33](https://github.com/NIWAFisheriesModelling/Casal2-supporting-information/raw/main/TestCases/CASAL/casal.Rtools42.MinGW.exe)
- [Linux executable for version 2.33](https://github.com/NIWAFisheriesModelling/Casal2-supporting-information/raw/main/TestCases/CASAL/casal)

Windows files
- [Windows installation package for version 2.30](https://github.com/NIWAFisheriesModelling/Casal2-supporting-information/raw/main/TestCases/CASAL/Setup_CASAL.exe)
- [Windows zip file for version 2.30](https://github.com/NIWAFisheriesModelling/Casal2-supporting-information/raw/main/TestCases/CASAL/CASALv230-2012-03-21.zip)
- [Windows zip file for version 2.33](https://github.com/NIWAFisheriesModelling/Casal2-supporting-information/raw/main/TestCases/CASAL/CASALv233-2022-08-04.zip)

CASAL R packages
- [CASAL R package for Windows](https://github.com/NIWAFisheriesModelling/Casal2-supporting-information/raw/main/TestCases/R-functions/casal_2.30.zip)
- [CASAL R package for Linux](https://github.com/NIWAFisheriesModelling/Casal2-supporting-information/raw/main/TestCases/R-functions/casal_2.30.tar.gz)

## CASAL version 2.33 was released on 2022-08-05

The CASAL executables for Windows and Linux includes bug fixes for:
- an issue with disease mortality being applied in the wrong timestep(s) (Craig Marsh)

In addition, CASAL versions 2.32 and newer have a new selectivity ogive, 'double_normal_stock_synthesis'. The CASAL ogive has 9 parameters, 6 that match the [Stock Synthesis 3](https://vlab.noaa.gov/web/stock-synthesis) implementation, and 3 additional parameters for the minimum bin value ("min_x_val", for age or size), the maximum bin value ("max_x_val", for age or size), and the bin width ("bin_width", which is usually 1 for age-based models). The latter 3 parameters should have the lower and upper bounds set to the parameter values so that they are not estimated.

NOTE: the CASAL manual has had no changes since version 2.30 released in 2012.

## CASAL version 2.31 was released on 2021-08-11

The CASAL executables for Windows and Linux includes bug fixes for:
 - an issue with tagging length bins (Craig Marsh);
 - an issue with two subcommands available for 'abundance' but not available for 'relative_abundance' (Alistair Dunn);
 - an issue with the sex-specific Schnute age-length relationship, which was previously using the female-specific relationship for both males and females; and
 - an issue with the covariance matrix and the maximum correlation check, and increasing the buffer sizes in the BetaDiff ADOL-C library.
