
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
| SOD08      |  Δq < -0.2            | Δq > 0.2        |        -          | z*<ABL*   |      Δq < -0.2    |     -          |  Sodemann et al. (2008)    |
|            |  RH > 80%             |                 |                   |           |                   |                |                            |
+------------+-----------------------+-----------------+-------------------+-----------+-------------------+----------------+----------------------------+
| FAS19      |  Δq < -0.1            | Δq > 0.1        |        -          | no        |      Δq < -0.1    |     -          |  Freme and Sodemann (2019) |
|            |  RH > 80%             |                 |                   |           |                   |                |                            |
+------------+-----------------------+-----------------+-------------------+-----------+-------------------+----------------+----------------------------+
| JK22       |  Δq < 0               | Δq > 0          |   |ΔRH| < 20      | z<ABL_max |      Δq < 0       |     -          |  Keune et al. (2022)       |
|            |  RH > 80%             |                 |                   |           |                   |                |                            |
+------------+-----------------------+-----------------+-------------------+-----------+-------------------+----------------+----------------------------+
| APA22      |  Δq < -0.1            | Δq > 0          |    -              | no        |      Δq < 0       |     -          | Pérez-Alarcón et al (2022) |
+------------+-----------------------+-----------------+-------------------+-----------+-------------------+----------------+----------------------------+


For a more detailed understanding of LATTIN, Please refer to 

.. note::

   Pérez-Alarcón, A.; Fernández-Alvarez, J.C.; Nieto, R.; Gimeno, L. (2024). LATTIN: A Python-based tool for Lagrangian atmospheric moisture and heat tracking. Software Impacts, 20, 100638. https://doi.org/10.1016/j.simpa.2024.100638

