---
layout: page
title: REIGN Dataset
---

**February 2020 REIGN Dataset: February 3rd, 2020**

**New Leaders**
  * Spasovksi (Macedonia)
  * Sommaruga (Switzerland)
  * Kabua (Marshall Islands)
  * Haitham ibn Tariq (Oman)
  * Giammattei (Guatemala)

  
**Key Elections**
  * None this month
    
**Version Updates (As of February 12th, 2020)**
  * **February 12th**: Fixed a bug in which leaders who began their tenure in 2020 were not fully captured beyond January. The current REIGN dataset reflects this fix. 
  * Updated precipitation (SPI) estimates using NOAA’s December 2019 PREC/L release (https://www.esrl.noaa.gov/psd/data/gridded/data.prel.html).
  * The methodology used for SPI projection beyond the NOAA measurements has changed since the last update. Previously, a single seasonal ARIMA model was used for every country. We now use an auto.arima function to fit the best model for each country during SPI forecasting.
  
Find the most current REIGN data [here](https://cdn.rawgit.com/OEFDataScience/REIGN.github.io/gh-pages/data_sets/REIGN_2020_2.csv) 

Find the most current REIGN update-blog [here](https://medium.com/the-die-is-forecast/international-elections-and-leaders-january-2020-update-e1347b5a7dc4?source=friends_link&sk=e53e9a7c869a6613a9139a7e7a75b4ec)

### Election and Leader lists (February 2020)

[Election List](https://cdn.rawgit.com/OEFDataScience/REIGN.github.io/gh-pages/data_sets/electionlist_2_20.csv)

[Leader List](https://cdn.rawgit.com/OEFDataScience/REIGN.github.io/gh-pages/data_sets/leaderlist_2_20.csv)

[Regime List](https://cdn.rawgit.com/OEFDataScience/REIGN.github.io/gh-pages/data_sets/regime_list.csv)
	
### Codebook and Technical Notes

[Codebook](https://cdn.rawgit.com/OEFDataScience/REIGN.github.io/gh-pages/documents/reign_codebook.pdf)

[Technical Notes](https://cdn.rawgit.com/OEFDataScience/REIGN.github.io/gh-pages/documents/reign_notes.pdf)


### Questions?

If you are unable to download the data, or have questions/inquiries, please contact Clayton Besaw (<cbesaw@oneearthfuture.org>). Also feel to contact Clayton if you notice any bugs or wrongly coded data. Thanks!

