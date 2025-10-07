# Near Surface Lapse Rate - Variability on Mount Washington

During my internship with the Mount Washington Observatory, I was tasked with completing a preliminary investigation into near surface lapse rate using in-situ data collected by the observatory. The results of the investigation are found in this repository. More detailed description of the methods and conclusions can be found in the project.ipynb file which I encourage you to read. 

## What is Near Surface Lapse Rate
Near Surface Lapse Rate refers to the rate at which air temperature changes with elevation within the first few meters above ground level—typically measured 2 meters above the surface. This metric is especially important in mountainous regions, where terrain influences airflow, solar heating, and surface cooling. Tracking lapse rates along elevation gradients helps scientists understand how temperature varies with altitude in complex terrain. These variations affect local microclimates, vegetation patterns, snowmelt timing, and wildlife habitats. Steeper lapse rates may indicate stronger cooling with altitude, which is vital for modeling heat transport, frost risk, and climate dynamics. Accurate near-surface lapse rates are also critical for improving weather forecasts and climate models in mountainous areas, where temperature can change rapidly over short distances. Additionally, they play a key role in understanding how climate change impacts high-elevation environments.

## Data and Availability
The Mount Washington Observatory has a network of remote weather stations, this includes an array of stations along the Mount Washington Auto-Road. This project uses 2016-2023 data of 7 measurements stations along the road, located at: 1600ft, 2300ft, 3300ft, 4000ft, 4300ft, 5300ft and at 6288ft. For those interested in applying the data for their own research needs, I encourage you to reach out to the Mount Washington Observatory about data sharing, collaboration, and research project opportunities. 

## Methods
This notebook applies fourier methods to investigate the variability of NSLR on the summit. Finding the normalized power spectra of both the temperature data and the NSLR (found using linear regression as per methodology guidelines). Hypotethis testing is validated using a 1-Dimensional Orstein Ulhenbeck process, with parameters estimated using autocorrelation functions of both the temperature data and the NSLR data. To address noise and degrees of freedom the data is windowed using the standard Hanning window. 

## Main Conclusions
Normalized PSD of temperature data across elevations exhibited a strong signal for seasonal frequencies, which NSLR exhibited the strongest signal in diurnal frequencies, with seasonal frequencies playing a second order role. From autocorrelations it was also found that temperature and NSLR behave fundamentally differently. This is an interesting conclusion and has possible applications in modelling and forecasting. 
