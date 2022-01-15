# EASAT-2 and HADES TLE lottery

This repository contains data files for the TLE identification of the EASAT-2
and HADES satellites from AMSAT-EA, which were launched on 2022-01-13 in the
SpaceX Transporter-3 launch.

The files are intended to be used with the [strf](https://github.com/cbassa/strf)
software.

## Logbook

### 2021-01-15 18:07 UTC - ATA observation

An observation with Allen Telescope Array has been done, detecting good signals
from EASAT-2 and a very weak signal that could be HADES. The `satnogs-2022-01-15-DELFI-PQ.tle` was used for tracking. This TLE was taken from
[a thread in the Librespace forums](https://community.libre.space/t/spacex-f9-transporter-3-2022-01-13-15-25utc/8776/51).

The Doppler data files corresponding to this observation are `2022-01-15_ATA_DELFI-PQ.dat`,
`2022-01-15_ATA_EASAT-2.dat` and `2022-01-15_ATA_HADES.dat`.

The `satnogs-2022-01-15-DELFI-PQ.tle` is a good match for all the three Doppler
data files. A fit in mean anomaly was done to try to judge the separation of the
three satellites in the along-track dimension. With
`satnogs-2022-01-15-DELFI-PQ.tle`, the predicted TCA for ATA of DELFI-PQ was
18:11:26. By doing a fit in mean anomaly we obtain TCA's of 18:11:35, 18:11:37
and 18:11:34 for DELFI-PQ, EASAT-2 and HADES.

The resulting TLEs obtained with this fit are
`AMSAT-EA-2022-01-15-DELFI-PQ.tle`, `AMSAT-EA-2022-01-15-EASAT-2.tle` and
`AMSAT-EA-2022-01-15-HADES.tle`. Observers are advised to use the
`satnogs-2022-01-15-DELFI-PQ.tle` instead of these, since it is based on data
from several passes.

The conclusion is that the three satellites are still close, and perhaps only
3-4 seconds apart at most. This data is relevant for the radiometric study of
the ATA data, since it suggest that all the satellites were present in the
primary beam of the antennas. A separation of 1 second is on the order of 0.8
deg separation on the sky at TCA on an overhead pass. The ATA FWHM at 436 MHz
is around 3.8 deg.
