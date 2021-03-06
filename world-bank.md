---
title: World Bank Data
description: An overview of the World Bank data holdings
---

The World Bank has a wide array of high quality data and much of it is [open data][]. It covers several distinct collections and databases.

* [Open Data Catalog][] - a listing of available World Bank datasets. You can browse from https://data.worldbank.org/

* [World Development Indicators][] - It includes over 15 major databases with more than 2000 indicators.

* [DataBank][] - collections of time series data on a variety of topics. Total: 69 databases.

* [Open finances][] - World Bank Group’s financials datasets such as
  * [Loans and credits][] - 5 datasets
  * [Financial Reporting][] - 23 datasets
  * [Shareholder Equity][] - 4 datasets
  * [Procurement][] - 4 datasets
  * [Projects][] - 9 datasets
  * [Budget][] - 3 datasets

* [Projects & operations][] - information on all of the World Bank's lending projects since 1947. Around 13,119 projects in 173 countries.

* [Global Consumption Database][] - datasets on household consumption patterns in developing countries. Data can be derived by country, sector or product.

* [Microdata Library][] - collection of sample surveys of households, business establishments or other facilities. As of April 02, 2018 the Library contains 2,503 surveys and 2,577 citations.

[Open Data Catalog]: http://datacatalog.worldbank.org/
[World Development Indicators]:https://data.worldbank.org/products/wdi
[DataBank]:http://databank.worldbank.org/data/home.aspx
[Open finances]:https://finances.worldbank.org/
[Loans and credits]:https://finances.worldbank.org/browse?category=Loans+and+Credits&limitTo=datasets
[Financial Reporting]:https://finances.worldbank.org/browse?category=Financial+Reporting&limitTo=datasets
[Shareholder Equity]:https://finances.worldbank.org/browse?category=Shareholder+Equity&limitTo=datasets
[Procurement]:https://finances.worldbank.org/browse?category=Procurement&limitTo=datasets
[Projects]:https://finances.worldbank.org/browse?category=Projects&limitTo=datasets
[Budget]:https://finances.worldbank.org/browse?category=Budget&limitTo=datasets
[Projects & operations]:http://projects.worldbank.org/
[Global Consumption Database]:http://datatopics.worldbank.org/consumption/
[Microdata Library]:http://microdata.worldbank.org/catalog
[open data]: https://opendefinition.org/

[[toc]]

## Data

We have created [world-bank](https://datahub.io/world-bank) user specifically for World Bank datasets, so they will be found in one place.

### World Development Indicators

One of the major open ones are the [World Development Indicators][] which provide a variety of important indicators ranging from GDP and population to CO2 emissions and literacy in a standardized cross country form. It consists of several main categories:

-   Agriculture & Rural Development

-   Aid Effectiveness

-   Climate Change

-   Economy & Growth

-   Education

-   Energy & Mining

-   Environment

-   External Debt

-   Financial Sector

-   Gender

-   Health

-   Infrastructure

-   Poverty

-   Private Sector

-   Public Sector

-   Science & Technology

-   Social Development

-   Social Protection & Labor

-   Trade

-   Urban Development

## API

The World Bank has a data API. You can use this to access a variety of data including the world development indicators.

You can get data in CSV, JSON and XML (default).

Per indicator:

```bash
https://api.worldbank.org/indicator/GC.DOD.TOTL.GD.ZS?format=csv

# for some reason json format just yields metadata
https://api.worldbank.org/indicator/GC.DOD.TOTL.GD.ZS?format=json
```

More elaborate queries documented in http://blogs.worldbank.org/opendata/first-steps-in-integrating-open-data, for example:

http://api.worldbank.org/en/countries/KE;XF;XM/indicators/EN.ATM.CO2E.PC?date=1961:2011&format=csv

http://api.worldbank.org/en/countries/KE;XF;XM/indicators/EN.ATM.CO2E.PC?date=1961:2011&format=json

### Scripts

Here is a script that automates access to World Bank data and conversion to data packages.

https://github.com/rufuspollock/world-bank-data


## License

License: OPEN (mostly)

Currently no easy way to automatedly obtain that listing though.

As of April 20th 2010 data is now open (subject to some reservations for specific datasets). See this [blog post](http://blog.okfn.org/2010/04/20/world-bank-opens-up-development-data/).

### License Details

[Terms of use summary](http://data.worldbank.org/summary-terms-of-use) state:

> You are free to copy, distribute, adapt, display or include the data in other products for commercial and noncommercial purposes at no cost subject to certain limitations summarized below.
> 
> You must include attribution for the data you use in the manner indicated in the metadata included with the data.
> 
> You must not claim or imply that The World Bank endorses your use of the data by or use The World Bank’s logo(s) or trademark(s) in conjunction with such use.
>
> Other parties may have ownership interests in some of the materials contained on The World Bank Web site. For example, we maintain a list of some specific data within the Datasets that you may not redistribute or reuse without first contacting the original content provider, as well as information regarding how to contact the original content provider. Before incorporating any data in other products, please check the list: Terms of use: Restricted Data
>
> The World Bank makes no warranties with respect to the data and you agree The World Bank shall not be liable to you in connection with your use of the data.

