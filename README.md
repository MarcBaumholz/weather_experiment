weather_experiment
------------------

This code can be used to investigate the [DWD (Deutsche Wetterdienst) weather forecasts](https://www.dwd.de/EN/ourservices/cdc/cdc_ueberblick-klimadaten_en.html) produced by MOSMIX(https://www.dwd.de/DE/leistungen/met_verfahren_mosmix/met_verfahren_mosmix.html).

Set up your environment by using Python:

```
python3.12 -m venv venv && source venv/bin/activate
pip install -r requirements.txt
```

We include one script for:

- [weather forecast aggregation via Google Cloud](./forecasts.py)
- [historical weather browsing](./historical_weather.py)

The stations used for this project are saved in [stations.txt](./stations.txt).
The stations need to be mapped from the [forecast identifiers](https://www.dwd.de/DE/leistungen/met_verfahren_mosmix/mosmix_stationskatalog.cfg?view=nasPublication&nn=16102) to the [real measuring station ids](https://opendata.dwd.de/climate_environment/CDC/help/zehn_min_tu_Beschreibung_Stationen.txt).
