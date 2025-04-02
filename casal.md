---
#layout: home
title: CASAL Files for Windows and Linux
permalink: /casal/
---

# CASAL

Casal2 is a next generation open-source integrated assessment tool for modelling the population dynamics of marine species, including fishery stock assessments. Casal2 expands functionality and increases maintainability relative to its predecessor, [CASAL](https://niwa.co.nz/fisheries/tools-resources/casal). Casal2 can be used for quantitative assessments of marine populations, including fish, invertebrates, marine mammals, and seabirds.

Casal2 is supported by Fisheries New Zealand, NIWA, Ocean Environmental Limited and Scott Rasmussen (Zaita) through the Casal2 Steering Group.

The Casal2 Development Team welcomes your contributions and feedback. Information about the use and development of Casal2 is available below.

## CASAL User Support and Community Forums

Please post questions about and issues with CASAL on [Slack](https://join.slack.com/t/casal2workspace/shared_invite/zt-2ko29a60h-jJpdINxi4OSb~tVNe0nRrQ).

## CASAL files for Windows and Linux

The latest version of Casal2 can be downloaded from Github [here](https://github.com/Casal2/CASAL2/releases).

## CASAL2 version 2024.06

CASAL2 received a bunch of code cleanup, minor fixes and updates.
- Added sqrt transformations to manual
- Added mortality constant exploitation process
- Implemented double tag loss
- Added disease mortaloty as an age model process
- Added constant difference parameter transformation

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
