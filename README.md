# yaPSAT EOV data

Daily sea surface temperatures and sunrise and sunset times for the yaPSAT R package.

## Data version 1

The 1° North Atlantic grid (`north_atlantic_1deg`) has 145 longitude cells and 80 latitude cells. The pilot covers 1 January 2017 through 31 December 2018. Arrays use longitude × latitude × day order. SST is in degrees Celsius.

The [version 1 manifest](https://github.com/baktoft/yapsat-eovs/releases/download/eov-v1/manifest.csv) lists asset names, inclusive date ranges, and SHA-256 checksums. The [releases page](https://github.com/baktoft/yapsat-eovs/releases) lists the annual files.

## Data sources

SST was sampled from the Copernicus Marine dataset `C3S-GLO-SST-L4-REP-OBS-SST` onto the yaPSAT grid. Generated using E.U. Copernicus Marine Service Information. [Product DOI](https://doi.org/10.48670/moi-00169).

Sunrise and sunset were computed from grid coordinates and calendar dates with the R package `suncalc`.
