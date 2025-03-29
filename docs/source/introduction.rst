
LATTIN: Lagrangian Atmospheric moisTure and heaT trackINg
=================================
The Lagrangian Atmospheric moisTure and heaT trackINg (LATTINv1.0.4) is a software developed in Python and Fortran
for the study of moisture and heat sources. It has been developed within the 
SETESTRELO project at the EPhysLab (Environmental Physics Laboratory) at the University of Vigo. 


.. image:: _static/LogoV1.png
   :alt: Logo de LATTIN
   :align: center
   :width: 400px


LATTIN is a Python-based tool for Lagrangian atmospheric moisture and heat tracking

Moisture tracking methods
-------------------------

dfdfdf

+------------+-----------------------+-------------------------------------------------+------------------------------------+----------------------------+
|            | Precipitating parcels |     **Moisture uptake**                         |      **Moisture losses**           |                            |
| **Method** | at target region      +-----------------+-------------------+-----------+-------------------+----------------+      **Reference**         |
|            |                       | **Δq (g/kg)**   | **|ΔRH| (%)**     | ABL       | **Δq (g/kg)**     | **RH (%)**     |                            |  
+------------+-----------------------+-----------------+-------------------+-----------+-------------------+----------------+----------------------------+
|  SJ05      |         -             |      -          |        -          |  no       |       -           |     -          |  Stohl and James (2005)    |
+------------+-----------------------+-----------------+-------------------+-----------+-------------------+----------------+----------------------------+
| SOD08      |  Δq < -0.2  &         | Δq > 0.2        |        -          | z*<ABL*   |      Δq < -0.2    |     -          |  Sodemann et al. (2008)    |
|            |  RH > 80%             |                 |                   |           |                   |                |                            |
+------------+-----------------------+-----------------+-------------------+-----------+-------------------+----------------+----------------------------+
| FAS19      |  Δq < -0.1  &         | Δq > 0.1        |        -          | no        |      Δq < -0.1    |     -          |  Freme and Sodemann (2019) |
|            |  RH > 80%             |                 |                   |           |                   |                |                            |
+------------+-----------------------+-----------------+-------------------+-----------+-------------------+----------------+----------------------------+
| JK22       |  Δq < 0  &            | Δq > 0          |    < 20           | z<ABL_max |      Δq < 0       |     -          |  Keune et al. (2022)       |
|            |  RH > 80%             |                 |                   |           |                   |                |                            |
+------------+-----------------------+-----------------+-------------------+-----------+-------------------+----------------+----------------------------+
| APA22      |  Δq < -0.1            | Δq > 0          |        -          | no        |      Δq < 0       |     -          | Pérez-Alarcón et al (2022) |
+------------+-----------------------+-----------------+-------------------+-----------+-------------------+----------------+----------------------------+


For a more detailed understanding of LATTIN, Please refer to 

.. note::

   Pérez-Alarcón, A.; Fernández-Alvarez, J.C.; Nieto, R.; Gimeno, L. (2024). LATTIN: A Python-based tool for Lagrangian atmospheric moisture and heat tracking. Software Impacts, 20, 100638. https://doi.org/10.1016/j.simpa.2024.100638



References
----------

Fremme, A. & Sodemann, H. (2019). The role of land and ocean evaporation on the variability of precipitation in the Yangtze River valley,
Hydrol. Earth Syst. Sci., 23, 2525-2540, https://doi.org/10.5194/hess-23-2525-2019.

Keune, J., Schumacher, D.L., Miralles, D.G. (2022). A unified framework to estimate the origins of atmospheric moisture
and heat using Lagrangian models. Geosci. Model Develop., 15(5), 1875-1898. Geosci. Model Dev., 15, 1875–1898.
https://doi.org/10.5194/gmd-15-1875-2022

Pérez-Alarcón A, Sorí R, Fernández-Alvarez JC, Nieto R, Gimeno L (2022). Where does the moisture for North Atlantic tropical 
cyclones come from?. J. Hydrometeorol., 23:457–472. https://doi.org/10.1175/JHM-D-21-0117.1.

Sodemann H, Schwierz C, Wernli H. (2008). Interannual variability of Greenland winter precipitation sources: 
Lagrangian moisture diagnostic and North Atlantic Oscillation influence. J. Geophys. Res.-Atmos.; 
113:D03107. https://doi.org/10.1029/2007JD008503.

Stohl A, James P A. (2005). A Lagrangian analysis of the atmospheric branch of the global water cycle: Part II:
Earth’s river catchments ocean basins, and moisture transports between them. J. Hydrometeorol., 6:961–984.
https://doi.org/10.1175/JHM470.1.