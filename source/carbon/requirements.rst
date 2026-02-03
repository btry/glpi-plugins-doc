.. list-table::
   :header-rows: 1

   * - Download
     - Sources
   * - `<https://github.com/pluginsGLPI/carbon/releases>`_
     - `<https://github.com/pluginsGLPI/carbon>`_

Requirements (on-premise)
-------------------------

============ =========== =========== ============
GLPI Version Minimum PHP Recommended Minimum DBMS
============ =========== =========== ============
10.0.19       8.2         8.2         Mysql 8.0 or MariaDB 10.2
============ =========== =========== ============
11.0.0        8.2         8.2         Mysql 8.0 or MariaDB 10.2
============ =========== =========== ============

It is mandatory to `enable timezones in GLPI <https://glpi-install.readthedocs.io/en/latest/timezones.html>` and set the timezone to the host for optimal execution. Not doing so will generate unnecessary HTTP requests to carbon intensitiy providers because of issues with DST handling.


.. warning:: For MySQL, a minimum version of 8.0 is required

.. include:: ../include/no_subscription_no_cloud.rst