Liste des esclaves EtherCAT
===========================

Cette page liste les esclaves découverts par la commande :

.. code-block:: bash

   ethercat slaves

.. tabs::

   .. tab:: Vue tableau

      .. csv-table:: Inventaire des esclaves
         :header: "#","Adresse","État","Type","Nom du périphérique"
         :widths: 5, 12, 12, 16, 55
         :file: _static/slaves.csv

   .. tab:: Vue terminal

      .. literalinclude:: _static/ethercat_slaves.txt
         :language: none

.. note::

   La **Vue tableau** est une version enrichie (traduite et typée) de la sortie terminal.
   La **Vue terminal** est la capture brute utilisée comme référence.

