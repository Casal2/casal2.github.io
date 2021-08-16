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

[CASAL User Manual for version 2.30](https://github.com/NIWAFisheriesModelling/CASAL2/blob/master/TestCases/CASAL/casalv230-2012-03-21.pdf)

Executable files
- [Windows executable for version 2.31](https://github.com/NIWAFisheriesModelling/CASAL2/blob/master/TestCases/CASAL/casal.exe)
- [Linux executable for version 2.31](https://github.com/NIWAFisheriesModelling/CASAL2/blob/master/TestCases/CASAL/casal)

Windows files
- [Windows installation package for version 2.30](https://github.com/NIWAFisheriesModelling/CASAL2/blob/master/TestCases/CASAL/Setup_CASAL.exe)
- [Windows zip file for version 2.30](https://github.com/NIWAFisheriesModelling/CASAL2/blob/master/TestCases/CASAL/CASALv230-2012-03-21.zip)

CASAL R packages (for use with R versions 3.6.X and older only)
- [CASAL R package for Windows](https://github.com/NIWAFisheriesModelling/CASAL2/blob/master/TestCases/CASAL/casal_2.30.zip)
- [CASAL R package for Linux](https://github.com/NIWAFisheriesModelling/CASAL2/blob/master/TestCases/CASAL/casal_2.30.tar.gz)

## CASAL version 2.31 was released on 2021-08-11

The CASAL executables for Windows and Linux includes bug fixes for:
 - an issue with tagging length bins (Craig Marsh);
 - an issue with two subcommands available for 'abundance' but not available for 'relative_abundance' (Alistair Dunn);
 - an issue with the sex-specific Schnute age-length relationship, which was previously using the female-specific relationship for both males and females; and
 - an issue with the covariance matrix and the maximum correlation check, and increasing the buffer sizes in the BetaDiff ADOL-C library.
