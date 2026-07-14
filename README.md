# Science Garden Rainfall Trends

This repository contains the data-processing and analysis workflow for a station-based rainfall trend study at PAGASA Science Garden, Quezon City, Philippines.

The study examines long-term changes in daily rainfall occurrence, seasonal accumulation, moderate-to-heavy rainfall frequency, and dry-spell persistence. The main analysis focuses on the Science Garden daily rainfall record, with particular attention to annual, November–April, and May–October rainfall behavior.

The workflow also includes sensitivity checks that separate all-days rainfall indices from indices calculated after masking days when a tropical cyclone (TC) centre was within 1000 km of Science Garden. These TC-proximity filters are used as diagnostic sensitivity tests only; they are not treated as formal rainfall attribution to tropical cyclones.

## Data availability

Raw rainfall and tropical cyclone best-track data are not distributed with this repository. Users who wish to reproduce or extend the analysis should obtain the required datasets directly from the original data providers.

### PAGASA Science Garden rainfall data

The Science Garden daily rainfall record used in this study was obtained from the Philippine Atmospheric, Geophysical and Astronomical Services Administration (PAGASA). These data are not redistributed in this repository. Users may request climatological data through the PAGASA Climate Data portal:

- [PAGASA Climate Data](https://www.pagasa.dost.gov.ph/climate/climate-data)

Users should follow PAGASA’s current data-request procedures, requirements, and terms of use.

### Tropical cyclone best-track data

Tropical cyclone proximity indicators were derived from the International Best Track Archive for Climate Stewardship (IBTrACS), provided by NOAA/NCEI. Users may download IBTrACS data from:

- [NOAA/NCEI International Best Track Archive for Climate Stewardship (IBTrACS)](https://www.ncei.noaa.gov/products/international-best-track-archive)

This study used the western North Pacific IBTrACS subset in CSV format.

### Expected local file structure

After obtaining the data, place the files locally using paths similar to:

```text
data/sci-garden-daily.csv
data/ibtracs.WP.list.v04r01.csv