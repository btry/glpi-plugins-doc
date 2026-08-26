Features
========

* Collect carbon intensity of electricity from various sources
  * RTE (France)
  * Electricity Map (most countries and regions of the whole world)
* Supports constant carbon intensity for the following regions
  * Quebec
* Fallbacks to yearly world carbon intensity if no data is available for the region of an asset
* Estimate consumed energy and carbon emission of assets
* Show results as charts

Supported assets
----------------

the table below describes how assets are supported by the plugin.

+-------------------+---------------+-----------+-----------+
|                   | Manufacturing |   Usage   | Recycling |
+===================+===============+===========+===========+
| Computer          |      Yes      |    Yes    |    No     |
+-------------------+---------------+-----------+-----------+
| Monitor           |      Yes      |    Yes    |    No     |
+-------------------+---------------+-----------+-----------+
| Network equipment |   User data   |    Yes    |    No     |
+-------------------+---------------+-----------+-----------+
| Smartphone        |      Yes      |    Yes    |    No     |
+-------------------+---------------+-----------+-----------+
| Tablet            |      Yes      |    Yes    |    No     |
+-------------------+---------------+-----------+-----------+

.. note:: RTE is free; ElectricityMaps is available with a subscription or with a very limitative free access

Features changelog
==================

Version 1.0.0 (for GLPI 10) and 1.1.0 (for GLPI 11)
---------------------------------------------------

  Support for 3 impact criteria
  * GWP (Global Warming Potential)
  * ADP (Abiotic Depletion Potential) (embodied only)
  * PE (Primary Energy) (embodied only)

Version 1.1.1 (GLPI 11)
-----------------------


Version 1.2.0
-------------

* Supports up to 20 impact criteria
* User defined impact values in asset models, taking precedence over 3rd party evaluation tools
* Supports paid access to ElectricityMaps

Version 1.3.0
-------------

* Per model user-defined impacts
* Diagnosis of carbon intensitiy data in cron tasks (view of gaps)