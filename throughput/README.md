# throughput
This directory contains model throughput data for the GOTO telescopes. See `throughput.ipynb` for some examples and plots.

Data files are stored in `/data`, either as individual elements or a combined CSV file (created by `throughput.ipynb`).

## GOTO filter properties

GOTO uses a Baader LRGBC set of filters (https://www.baader-planetarium.com/en/filters/filter-sets/baader-l-rgb-c-ccd-filterset.html). C is clear glass, and is not used for observing.

![Throughput plot](throughput.png)

The values in this table (and the plot above) are output by  `throughput.ipynb`.

| Filter | Midpoint | Bandwidth | Throughput (no atm) |
| - | - | - | - |
| L | 5469 Å | 2536 Å | 0.4546 e-/ph |
| R | 6449 Å |  963 Å | 0.4261 e-/ph |
| G | 5371 Å |  911 Å | 0.5112 e-/ph |
| B | 4532 Å | 1066 Å | 0.3711 e-/ph |

The values in this table are output by `synphot.ipynb`. Sky fluxes are in e-/s/cm²/arcsec². The 5-sigma limiting magnitude is for a single 120s exposure in a dark sky, at airmass 1 and with seeing of 1.5.

| Filter | Zeropoint </br> (AB mag) | Zeropoint </br> (Vega mag) | Dark sky flux  | Grey sky flux | Bright sky flux | Extinction | Limiting mag |
| - | - | - | - | - | - | - | - |
| L | 22.63 | 22.62 | 0.0031 | 0.0173 | 0.0331 | 0.148 mag | 19.76 |
| R | 21.33 | 21.14 | 0.0014 | 0.0051 | 0.0096 | 0.099 mag | 18.55 |
| G | 21.67 | 21.68 | 0.0012 | 0.0070 | 0.0139 | 0.144 mag | 18.85 |
| B | 21.66 | 21.78 | 0.0007 | 0.0070 | 0.0131 | 0.215 mag | 18.78 |