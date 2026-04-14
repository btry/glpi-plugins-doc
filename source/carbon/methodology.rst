Methodology
===========

Embodied impacts
----------------

The methodology of embodied impact is directly inherited from the external engine used.

Carbon uses the characteristics of assets and its the components (for computers) to describe the asset with repect of expectations of the external engine.

Boaviztapi
^^^^^^^^^^

Boaviztapi is a tool produced by Boavizta, an association helping organizations to assess, manage and reduce the environmental impact of their digital assets in a simple, fast and reliable way.

The Carbon plugin sends queries to this tool to get metrics which are locally saved and agregated.

Usage impacts
-------------

The plugin internally calculates the emissions of carbon dioxide equivalent, using the carbon intensity of the local electricity supplier of each asset. Other impacts are calculated by the external tool enabled in the plugin.

Greenhouse gas emissions
^^^^^^^^^^^^^^^^^^^^^^^^

The Carbon plugin identifies the location of an asset, the average power consumption and theorical power-on and power-off times to approximate the amount of greenhouse gas emitted by the asset's usage.

The carbon intensity of electricity is collected from local providers and down-sampled to 1 hour time slots. For each asset where there is enough data, the plugin evaluates when it is powered on and calculates the average energy consumed then the carbon emissions of this energy consumption.

When the data source for the location does not provide carbon intensity or when there is no real time data source availabie, the plugin seearches for fallback data in its internal database of yearly carbon intensity per contry. This data comes from https://ourworldindata.org/grapher/carbon-intensity-electricity .

The results are then aggregated by day, and are used to calculate the total carbon emission on a larger time frame, like a month or a year.