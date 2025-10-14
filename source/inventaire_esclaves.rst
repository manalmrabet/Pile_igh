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


Support des horloges distribuées (DC)
-------------------------------------

Les informations ci-dessous sont extraites de ``ethercat slaves -v`` (champ
``Distributed clocks`` et ``DC system time transmission delay``).

.. list-table:: **Support DC et délai de transmission**
   :header-rows: 1
   :widths: 8 28 18 18 28

   * - Adresse
     - Périphérique
     - DC
     - Résolution
     - Délai DC (ns)
   * - 0:0
     - EPOS3 70/10 EtherCAT
     - Oui
     - 64 bits
     - 0
   * - 0:1
     - EK1100 EtherCAT-Koppler (2A E-Bus)
     - Oui
     - 64 bits
     - 610
   * - 0:2
     - EL5101 1K. Inc. Encoder 5V
     - Oui
     - 64 bits
     - 755
   * - 0:3
     - EL4132 2Ch. Ana. Ausgang ±10V, 16 bits
     - Oui
     - 64 bits
     - 900
   * - 0:4
     - EL3102 2K. Ana. Eingang ±10V, Diff.
     - Oui
     - 64 bits
     - 1045
   * - 0:5
     - EL2008 8K. Dig. Ausgang 24V, 0.5A
     - Oui
     - 64 bits
     - 1185
   * - 0:6
     - EL1018 8K. Dig. Eingang 24V, 10µs
     - Oui
     - 64 bits
     - 1340

.. tip::

   Tous les esclaves de cette maquette reportent **``Distributed clocks: yes, 64 bit``**.
   Le champ **``DC system time transmission delay``** donne le décalage (ns) utilisé
   pour la compensation temporelle en topologie ligne/anneau.



