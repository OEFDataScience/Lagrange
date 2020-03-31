---
layout: page
title: REIGN Archive
---

Please find past REIGN data and update-blogs here:

**March 2020 REIGN Dataset: March 3rd, 2020**

**New Leaders**
  * Kurti (Kosovo)
  * Embalo (Guinea-Bissau)
  
**Key Elections**
  * Ireland (coalition talks on-going)
  * Slovakia (coalition talks on-going)
  * Togo (incumbent win, no leader change)
    
**Version Updates (As of March 6th, 2020)**
  * Fixed coding error in which Paraguay's leadership change in 2018 was not accounted for. 
  * Updated precipitation (SPI) estimates using NOAA’s December 2020 PREC/L release (https://www.esrl.noaa.gov/psd/data/gridded/data.prel.html).
  * Removed Tawfiq-Allawi (Iraq) as a leader following the withdrawal of his nomination earlier this month.
  * Fixed miscoding of start date for James Marape in Papua New Guinea. This fixed a bug in which Marape's tenure as PNG leader was not captured in the data.
  * Fixed coding bug concerning Raul Casto. We had originally replaced Castro as leader with Diaz-Canel. However, we changed the coding back to Raul Castro after digging deeper into the Cuban political structure. When this occured, we failed to remove the exit date information for Raul Castro, effectively removing Cuba from the data for 2019/2020.

  [Dataset](https://www.dl.dropboxusercontent.com/s/970g10a3seivdzg/REIGN_2020_3.csv?dl=0)
  
  [REIGN Update Blog](https://medium.com/the-die-is-forecast/international-elections-and-leaders-march-2020-briefing-b6664e7334ef)
  
**February 2020 REIGN Dataset: February 3rd, 2020**

**New Leaders**
  * Spasovksi (Macedonia)
  * Sommaruga (Switzerland)
  * Kabua (Marshall Islands)
  * Haitham ibn Tariq (Oman)
  * Giammattei (Guatemala)

  
**Key Elections**
  * None this month

  [Dataset](https://www.dl.dropboxusercontent.com/s/un9cke9u8oa4olu/REIGN_2020_2.csv?dl=0) 

  [REIGN Update Blog](https://medium.com/the-die-is-forecast/international-elections-and-leaders-february-2020-update-e6f58cddedd1)
 
    
**Version Updates (As of February 12th, 2020)**
  * **February 12th**: Fixed a bug in which leaders who began their tenure in 2020 were not fully captured beyond January. The current REIGN dataset reflects this fix. 
  * Updated precipitation (SPI) estimates using NOAA’s December 2019 PREC/L release (https://www.esrl.noaa.gov/psd/data/gridded/data.prel.html).
  * The methodology used for SPI projection beyond the NOAA measurements has changed since the last update. Previously, a single seasonal ARIMA model was used for every country. We now use an auto.arima function to fit the best model for each country during SPI forecasting.

**January 2020 REIGN Dataset: January 8th, 2020**

**New Leaders**
  * Fernandez (Argentina)
  * Sanna Marin (Finland)
  * Tebboune (Algeria)
  * Hassan Diab (Lebanon)

  
**Key Elections**
  * Guinea-Bissau (Presidential)
  * Papua New Guinea (Referendum)
  * United Kingdom (Legislative)
  * Algeria (Presidential)
  * Dominica (Legislative)
  * San Marino (Legislative)
  
  [Dataset](https://www.dl.dropboxusercontent.com/s/0vwlepc6t6jz8tj/REIGN_2020_1.csv?dl=0) 

  [REIGN Update Blog](https://medium.com/the-die-is-forecast/international-elections-and-leaders-january-2020-update-e1347b5a7dc4?source=friends_link&sk=e53e9a7c869a6613a9139a7e7a75b4ec)

    
**Version Updates (As of January 8th, 2020)**
  * No technical updates beyond new leaders and elections this month. All other predictors are using most up-to-date information.

**December 2019 REIGN Dataset: December 2nd, 2019**

**New Leaders**
  * Ion Chicu (Moldova)
  * Gotabaya Rajapaksa (Sri Lanka)

  
**Key Elections**
  * Mauritius 
  * Romania
  * Sri Lanka
  * Marshall Islands
  * Namibia 
  * Guinea-Bissau
  * Uruguay

    
**Version Updates (As of December 2nd, 2019)**
  * No technical updates beyond new leaders and elections this month. All other predictors are using most up-to-date information.
  * The REIGN team has changed how the current leader and elections lists are stored. They are now stored directly into the GitHub repository for easier automation access. The stored files will follow the same naming pattern (ex: leaderlist_"2digitmonth"_"last2digityear".csv)
  * Archived versions of the leaderlist, electionlist and REIGN are available by request from our organizational Dropbox.
  
	[Dataset](https://www.dl.dropboxusercontent.com/s/7hsdbi696si0tpb/REIGN_2019_12.csv?dl=0) 

	[REIGN Update Blog](https://oefresearch.org/news/international-elections-and-leaders-december-2019-update)

## November 2019

**New Leaders**
  * Luca Boschi and Mariella Mularoni (San Marino)
  * Sophie Wilmès (Belgium)
  * Pohiva Tu'i'onetoa (Tonga)
  * Kais Saied (Tunisia)
  
**Key Elections**
  * Argentina
  * Bolivia
  * Botswana
  * Canada
  * Kosovo
  * Mozambique
  * Switzerland
  * Tunisia
  * Uruguay

    
**Version Updates (As of November 6th, 2019)**
  * An acting PM for Tonga has been retroactively added to account for their leadership tenure before October's selection of a new PM.
  * Leadership in Cuba has been retroactively changed back to Raul Castro after examining the current leadership structure in Cuba. 
  * The coalition talks have been resolved in Belgium. Sophie Wilmès is now the first female prime minister in Belgian history.
  * Updated precipitation (SPI) estimates using NOAA's October 2019 PREC/L release (https://www.esrl.noaa.gov/psd/data/gridded/data.prel.html). 
  * Updated economic estimates with the IMF's October Global Economic Outlook release (https://www.imf.org/en/Publications/WEO/Issues/2019/10/01/world-economic-outlook-october-2019).
  * Updated economic estimates with the World Bank's newest GDP data (https://data.worldbank.org/indicator/ny.gdp.pcap.cd)
  * Updated infant mortality rate estimates with the World Bank's newest IMF data (https://data.worldbank.org/indicator/SP.DYN.IMRT.IN)
  * Updated internal political violence indicator using the newest Global Terrorism Database release (https://www.start.umd.edu/research-projects/global-terrorism-database-gtd)
  * Updated internal political violence indicator using newest UCDP Georeferenced Event Data release (https://ucdp.uu.se/downloads/)
  * Updated regime type for Bolivia. Bolivia is now coded as a party-personalist government as of October 25th, 2019. This was a difficult decision and the REIGN team waited until after the election to come to a conclusion. Given the government's behavior in previous term-limit debates and solid evidence of electoral irregularities, we have changed Bolivia from a presidential democracy to a party-personalist system. 

 [Dataset](https://www.dl.dropboxusercontent.com/s/0fviw46ak8vh6rf/REIGN_2019_11.csv?dl=0)
  
 [REIGN Update Blog](https://oefresearch.org/news/international-elections-and-leaders-november-2019-update)

## October 2019

**New Leaders**
  * Giorgi Gakharia (Georgia)
  * Kausea Natano (Tuvalu)
  
**Key Elections**
  * Afghanistan
  * Austria
  * Tunisia 
  * Tuvalu

    
**Version Updates (As of October 1st, 2019)**
  * Fixed leader election dates and national election outcomes related to the following leadership-country periods: Guyana 1964;1968, Paraguay 1989, Belgium 1995, Luxembourg 1954, Andorra 1985, West Germany Kissinger;Schdmit, Czechlosovakia 1990, Greece 1958;1961, Bulgaria 1949;1953-1986, Estonia 2007;2015, Latvia 2006, Armenia Kocheryan, Azerbaijan 1993; Finland 1982, Norway Torp, Iceland 1959, Mali 1974, Benin 1991;1996;2001;2006;2016, Guinea 1968;1974;1990;2001, Seychelles 2006;2015-2016, Sudan 1958, Israel Bengurion;Sharrett, Turkmenistan 2007; Tajikistan 1991;1994, South Korea 1979;1980, Myanmar Unu;Ubaswe, Sri Lanka 1952, Cambodia 1976;1998, Australia 1966;1975, Tuvalu 2004;2010 
  * Coalition outcome for Belgian general election is expected to take time, so the result is uncoded as of this update. (September Update: Looks like Belgium is in for a long caretaker period. If nothing changes, expect a PM change in December 2019 due to Michel's new commitments to the European Council). 
  * Updated precipitation (SPI) estimates using NOAA's August 2019 PREC/L release (https://www.esrl.noaa.gov/psd/data/gridded/data.prel.html). 
  * Updated regime type for Sudan. Sudan is now coded as a Civilian Provisional government as of August 2019. The REIGN team waited a month after the adoption of the Sovereignty Council of Sudan before making the decision. While the council will be headed by the military for the first 39 months of the transition, it lays the groundwork for civilian rule. 

 [Dataset](https://www.dl.dropboxusercontent.com/s/d9ndc3p6fr83eo4/REIGN_2019_10.csv?dl=0)
  
 [REIGN Update Blog](https://oefresearch.org/news/international-elections-and-leaders-october-2019-update)

## September 2019

**New Leaders**
  * Mohamed Ould Ghazouani (Mauritania)
  * Lionel Aingimea (Nauru)
  
**Key Elections**
  * Guatemala
  * Nauru

    
**Version Updates (As of September 3rd, 2019)**
  * Hotfix implemented to detect and correct "blank" country names in the first month of tenure for the following leaders: De Roburt (Nauru), Nakyama (Micronesia), Pashinyan (Armenia), da Costa (Sao Tome), Lini (Vanautu), Remeliik (Paulau). Hotfix will dynamically fix any problems with missing country names for future leaders. 
  * Coalition outcome for Belgian general election is expected to take time, so the result is uncoded as of this update. (September Update: Looks like Belgium is in for a long caretaker period. If nothing changes, expect a PM change in December 2019 due to Michel's new commitments to the European Council). 
  * Updated precipitation (SPI) estimates using NOAA's July 2019 PREC/L release (https://www.esrl.noaa.gov/psd/data/gridded/data.prel.html). 

 
 [Dataset](https://www.dl.dropboxusercontent.com/s/yfprg6uv9e6z2le/REIGN_2019_9.csv?dl=0)
  
 [REIGN Update Blog](https://oefresearch.org/news/international-elections-and-leaders-september-2019-update)
 


## August 2019

**New Leaders**
  * Laurentino Cortizo (Panama)
  * Kyriakos Mitsotakis (Greece)
  * Gitanas NausÄ—da (Lithuania)
  * Boris Johnson (United Kingdom)
  * Mohamed Ennaceur (Tunisia)
  
**Key Elections**
  * Greece

    
**Version Updates (As of July 30th, 2019)**
  * Identified a number of leaders (DeRoburt, Da Costa, Nakyama, Lini, Remeliik, Pashinyan) who do not have country codings for the first month of their tenure. This is an unexpected bug in the leader panel creation process and is currently being worked on.
  * Coalition outcome for Belgian general election is expected to take time, so the result is uncoded as of this update. 
  
  
 [Dataset](https://www.dl.dropboxusercontent.com/s/suu1l79owwkrrdx/REIGN_2019_8.csv?dl=0)
  
 [REIGN Update Blog](https://oefresearch.org/news/international-elections-leaders-august-2019)
 
 [CoupCast Update Blog](https://medium.com/the-die-is-forecast/august-2019-coupcast-mini-update-5cf2a65eb66d)

## July 2019

**New Leaders**
  * Nayib Bukele (El Salvador)
  * Mette Frederiksen (Denmark)
  * Antti Rinne (Finland)
  * James Merape (Papua New Guinea)
  * Pavel Filip/Maia Sandu (Moldova - Contested due to Constitutional Crisis)
  
**Key Elections**
  * Denmark
  * Guatemala
  * Kazakhstan
  * Mauritania

    
**Version Updates (As of July 2nd, 2019)**
  * Identified a number of leaders (DeRoburt, Da Costa, Nakyama, Lini, Remeliik, Pashinyan) who do not have country codings for the first month of their tenure. This is an unexpected bug in the leader panel creation process and is currently being worked on.
  * Pavel Filip and Maia Sandu both switch head executive status twice during the month of June in the REIGN dataset. This isn't perfect, but it is difficult to code leadership shifts within a constitutional crisis. This coding may change based on future information. 
  * Coalition outcome for Belgian general election is expected to take time, so the result is uncoded as of this update. 
  * Updated precipitation (SPI) estimates using NOAA's May 2019 PREC/L release (https://www.esrl.noaa.gov/psd/data/gridded/data.precl.html).
  
 [Dataset](https://www.dl.dropboxusercontent.com/s/3tw3159ayp56o8z/REIGN_2019_7.csv?dl=0)
  
 [REIGN Update Blog](https://oefresearch.org/news/international-elections-and-leaders-july-2019-update)
 
 [CoupCast Update Blog] - None for July due to vacation


## June 2019

**New Leaders**
  * Panuelo (Micronesia)
  * Xavier Espot Zamora (Andorra)
  * Hartwig Löger (Austria)
  * Brigitte Bierlein (Austria)
  * Zelensky (Ukraine)
  
**Key Elections**
  * Australia
  * Belgium
  * Lithuania
  * Malawi
  * Panama
  * South Africa
  * India

**Version Updates (As of June 3rd, 2019)**
  * Corrected leadership change for Australia to Morrison. This was not originally changed in August 2018. 
  * Coalition outcome for Belgian general election is expected to take time, so the result is uncoded as of this update.
  * Election outcome for Thailand currently unknown, so the result is uncoded as of this update. 
  * Finalized outcome data is coded for Andorra, Finland, and Indonesia.
  * Updated precipitation (SPI) estimates using NOAA's April 2019 PREC/L release (https://www.esrl.noaa.gov/psd/data/gridded/data.precl.html).
  
 [Dataset](https://www.dl.dropboxusercontent.com/s/gzm78kq6w1nriri/REIGN_2019_6.csv?dl=0)
  
 [REIGN Update Blog](https://oefresearch.org/news/international-elections-and-leaders-june-2019-update)
 
 [CoupCast Update Blog](https://medium.com/the-die-is-forecast/june-2019-coupcast-update-1deeff8a5907)

## May 2019

**New Leaders**
  * Assoumani (Comoros)
  * Changing of the Captains Regents (San Marino)
  * Ahmed Awad Ibn Auf (Sudan)
  * Abdel Fattah Abdelrahman Burhan (Sudan)
  * Manasseh Sogavare (Solomon Islands)
  * Abdelkader Bensalah (Algeria)
  
**Key Elections**
  * Andorra
  * Finland
  * Indonesia
  * Solomon Islands
  * Ukraine
  * Israel
  * Egypt (Referendum)
  * Spain
  
  
**Version Updates (As of May 1st, 2019)**
  * Fixed election outcome information for Estonia 2019 as coalition outcome was previously unclear. 
  * Preliminary outcome data is coded for Andorra, Finland, and Indonesia. These may change. 
  * Changed regime type for Sudan to military provisional.
  * Changed regime type for Algeria to civilian provisional.
  * Changed regime type for Egypt to military personalist. 
  * Updated precipitation (SPI) estimates using NOAA's March 2019 PREC/L release (https://www.esrl.noaa.gov/psd/data/gridded/data.precl.html).
  * Updated GDP and population data using the April 2019 IMF world economic outlook release (https://www.imf.org/external/pubs/ft/weo/2019/01/weodata/index.aspx).
  * Updated GDP using the newest World Bank release (https://data.worldbank.org/indicator/ny.gdp.mktp.cd).
  * Updated infant mortality rate data with newest World Bank release (https://data.worldbank.org/indicator/sp.dyn.imrt.in). Implemented country-specific ARIMA modeling for forecasting mortality rate for unreleased years. These numbers were previously produced using forward filling for unknown years. 
  * Added coup events in Sudan and Venezuela. 
  * Changed regime type for Turkey to party-personal hybrid (May 6th 2019) based on annulment of mayoral elections on May 6th. 
  
 [Dataset](https://www.dl.dropboxusercontent.com/s/ui9t0uysugrhqat/REIGN_2019_5.csv?dl=0)
  
 [REIGN Update Blog](https://oefresearch.org/news/international-elections-and-leaders-may-2019-update)
 
 [CoupCast Update Blog](https://medium.com/the-die-is-forecast/may-2019-coupcast-update-244d731e9d6f)

## April 2019

**New Leaders**
  * Kassym-Joymart Tokayev (Kazakhstan)
  * Abdelkader Bensalah (Algeria)
  
**Key Elections**
  * Estonia
  * North Korea
  * Thailand
  * Comoros
  * Micronesia
  
  
**Version Updates (As of April 9th, 2019)**
  * Tuvalu 2019 election deadline fixed.
  * Retroactively added Afghanistan December 2018 election delay/voiding.
  * Changed North Korea election type from executive to legislative.
  * Updated precipitation (SPI) estimates using NOAA's Jan 2019 PREC/L release (https://www.esrl.noaa.gov/psd/data/gridded/data.precl.html)
  * Corrected Israel's election date for April and announcement of early election in December 2018. 

 [Dataset](https://www.dl.dropboxusercontent.com/s/w2lebo0yttyadef/REIGN_2019_4.csv?dl=0)
  
 [REIGN Update Blog](https://oefresearch.org/news/international-elections-and-leaders-april-2019-update)
 
 [CoupCast Update Blog](https://medium.com/the-die-is-forecast/april-2019-coupcast-update-14ae895e8031)

## March 2019

**New Leaders**
  * Abdou (Comoros)
  
**Key Elections**
  * Cuba
  * El Salvador
  * Moldova
  * Nigeria
  * Senegal
  
**Version Updates (As of March 1st, 2019)**
  * Fixed Comoros presidential election dates/sequences. 
  * Fixed spelling of Canada country name. 
  * Fixed duplicate leader-month rows for Colombia.
  * Fixed duplicate leader-month rows for Armenia.
  * Added regularly accessible regime type data for download and for the [democracyData R package](https://github.com/xmarquez/democracyData)
  
 [Dataset](https://www.dl.dropboxusercontent.com/s/dx6inv008343r9c/REIGN_2019_3.csv?dl=0)
  
 [REIGN Update Blog](https://oefresearch.org/news/international-elections-and-leaders-march-2019-update)
 
 [CoupCast Update Blog](https://medium.com/the-die-is-forecast/march-2019-coupcast-update-79a3dbe0f224)

## February 2019

**New Leaders**
  * Karins (Latvia)
  * Rajoelina(Madagascar)
  * Tschisekedi (Demcoratic Republic of Congo)
  
**Key Elections**
  * None in January
  
**Version Updates (As of February 7th, 2019)**
  * Fixed a number of wrongly coded election outcomes.
  * Fixed a bug in leadership transition data regarding Liberia that caused duplicate leader-month rows.
  * Updated precipitation projections with December 2018 NOAA PREC/L numbers.
  * Updated armed conflict event data for new onsets and previous conflict termination. 
  * Added new coup event in Gabon - January 2019. 
  
 [Dataset](https://www.dl.dropboxusercontent.com/s/gwv6bgpmr02dqth/REIGN_2019_2.csv?dl=0)
  
 [REIGN Update Blog](https://oefresearch.org/news/international-elections-and-leaders-february-2019-update)
 
 [CoupCast Update Blog](https://medium.com/the-die-is-forecast/february-2019-coupcast-update-b89ce3b06489)

## January 2019

**New Leaders**
  * Obrador (Mexico)
  * Maurer (Switzerland)
  * Bakhtadze (Georgia)
  * Bolsonero (Brazil)
  
**Key Elections**
  * Armenia
  * Bangladesh
  * Democratic Republic of Congo
  * Madagascar
 
  [Dataset](https://www.dl.dropboxusercontent.com/s/aqppeo7hnavg3xs/REIGN_2019_1.csv?dl=0)
  
  [Blog](https://oefresearch.org/news/international-elections-and-leaders)

## December 2018

**Key Events**
  * Madagascar
  * Fiji
  * Nepal
  * Maldives
 
  [Dataset](https://www.dl.dropboxusercontent.com/s/o2vhc3bcncy3qxb/REIGN_2018_12.csv?dl=0)
  
  [Blog](http://oefresearch.org/news/international-elections-and-leaders-december-2018-update)
 
## November 2018

**Key Events**
  * Brazil
  * Bhutan
  * Bosnia and Herzegovina
  * Cameroon
  * San Marino
  
  [Dataset](https://www.dl.dropboxusercontent.com/s/41xam1136ha5c3j/REIGN_2018_11.csv?dl=0)
  
  [Blog](http://oefresearch.org/news/international-elections-and-leaders-november-2018-update)

## October 2018

**Key Events**
  * Madagascar
  * Slovenia
  * Bhutan
  * Maldives
  * Sweden
  
  [Dataset](https://www.dl.dropboxusercontent.com/s/lxq3haayz9b959j/REIGN_2018_10.csv?dl=0)
  
  [Blog](http://oefresearch.org/news/international-elections-and-leaders-october-2018-update)

## September 2018

**Key Events**
  * Mali
  * Ivan Duque (Colombia)
  * Imran Khan (Pakistan)
  
  [Dataset](https://www.dl.dropboxusercontent.com/s/xslos28ralqj3an/REIGN_2018_9.csv?dl=0)
  
  [Blog](http://oefresearch.org/news/international-elections-and-leaders-september-2018-update)

## August 2018

**Key Events**
  * Zimbabwe
  * Mali
  * Comoros 
  * Mexico
  * Pakistan
  * Cambodia
  
[Dataset](https://www.dl.dropboxusercontent.com/s/4m3k4n0l8t7ia0m/REIGN_2018_8.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-august-2018-update)

## July 2018

**Key Events**
  * Erdogan (Turkey)
  * Giuseppe Conte (Italy)
  * Sanchez (Spain)
  * Duque (Colombia)
  * Slovenia Parliamentary Election

[Dataset](https://www.dl.dropboxusercontent.com/s/s73agb5onpbehsb/REIGN_2018_7.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-july-2018)

## June 2018

**Key Events**
  * Muqtada al-Sadr (Iraq)
  * Hezbollah (Lebanon)
  * Nikol Pashinyan (Armenia)
  * Mia Mottley (Barbados)
  * Colombian Presidential Runoff
 
[Dataset](https://www.dl.dropboxusercontent.com/s/1h2wo6bzb1njj4y/REIGN_2018_6.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-june-2018-update)

  

## May 2018

**Key Events**
  * Sargsyan (Armenia)
  * Quesada (Costa Rica)
  * Orban (Hungary)
  * Abiye Ahmed (Ethiopia)
  * Julius Maada Bio (Sierra Leone)

[Dataset](https://www.dl.dropboxusercontent.com/s/dm49t8yp6byec5b/REIGN_2018_5.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-may-2018-update)


## April 2018

**Key Events**
  * Abdel-Fattah El-Sisi (Egypt)
  * Sebastian Piñera (Chile)
  * Martin Viscarra (Peru)
  * Cuba Election
  * Italy Election
  * Russia Election
  
[Dataset](https://www.dl.dropboxusercontent.com/s/xbrruywjpuxmbxr/REIGN_2018_4.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-leaders-april-2018-update)


## March 2018

**Key Events**
  * Jacob Zuma
  * Nepalese Parliament
  * Ecuadorian Referendum
  
[Dataset](https://www.dl.dropboxusercontent.com/s/8h5yrd16k6oiwsa/REIGN_2018_03.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-march-2018-update)

## February 2018
 
**Key Events**

  * George Weah
  * Cyprus Election

[Dataset](https://dl.dropboxusercontent.com/s/nupy5jgp1g7cpba/REIGN_2018_02.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-february-2018-update)

**note**: February 2018 is deprecated and will not be corrected. We apologize for any inconvenience. Please 
utilize March 2018 and beyond.

## January 2018 

**Key Events**

  * Sebastian Kurz, Andrej Babis, Alain Berset
  * Liberia Election
  * Chile Election

[Dataset](https://dl.dropboxusercontent.com/s/bca4i7wcuakf13i/REIGN_2018_01.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-january-2018-update)

## December 2017

[Dataset](https://dl.dropboxusercontent.com/s/iq5r4gvlnlklnfi/REIGN_2017_12.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-december-2017-update)

## November 2017

[Dataset](https://dl.dropboxusercontent.com/s/3c1vgdjsx6v2m5s/REIGN_2017_11.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-november-2017-update)

## October 2017

[Dataset](https://dl.dropboxusercontent.com/s/snb0dpmklasfh04/REIGN_2017_10.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-october-2017-update)

## September 2017

[Dataset](https://dl.dropboxusercontent.com/s/rjomdvg9uuzcae7/REIGN_2017_09.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-september-2017-update)

## August 2017

[Dataset](https://dl.dropboxusercontent.com/s/lvt35qq7xkzyxem/REIGN_2017_08.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-august-2017-update)

## July 2017

[Dataset](https://dl.dropboxusercontent.com/s/6c8z3pf67ckbp0q/REIGN_2017_07.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-july-2017-update)

## June 2017

[Dataset](https://dl.dropboxusercontent.com/s/u3b3uv28uafbk56/REIGN_2017_06.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-june-2017-update)

## May 2017

[Dataset](https://dl.dropboxusercontent.com/s/szhhhkfx6m7nicx/REIGN_2017_05.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-may-2017-update)

## April 2017

[Dataset](https://dl.dropboxusercontent.com/s/4t8tysgssepd9ne/REIGN_2017_04.csv?dl=0)

[Blog](http://oefresearch.org/news/international-elections-and-leaders-april-2017-update)

## March 2017

[Dataset](https://dl.dropboxusercontent.com/s/5wtpd022t7aonzo/REIGN_2017_03.csv?dl=0)

## February 2017

[Dataset](https://dl.dropboxusercontent.com/s/rtx7ec5hpwcjfh8/REIGN_2017_02.csv?dl=0)

## January 2017

[Dataset](https://dl.dropboxusercontent.com/s/tsn50pmx9p1pghe/REIGN_2017_01.csv?dl=0)

## December 2016

[Dataset](https://dl.dropboxusercontent.com/s/zt6is35wsojk1bn/REIGN_2016_12.csv)

## November 2016

**note**: Link deprecated

[Dataset](https://dl.dropboxusercontent.com/u/6884339/REIGN_2016_11.csv)

## October 2016

**note**: Link deprecated

[Dataset](https://dl.dropboxusercontent.com/u/6884339/REIGN_2016_10.csv)









