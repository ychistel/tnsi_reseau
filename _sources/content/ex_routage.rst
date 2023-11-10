Exercices : protocoles RIP et OSPF
==================================

Exercice 1
----------

On considère le réseau composé de 4 routeurs A, B , C et D reliés selon le graphe ci-dessous:

.. figure:: ../img/graphe_reseau_2.svg
   :align: center
   :width: 320

Le protocole RIP est utilisé au sein de ce réseau.

#. Dresser la table de routage de chaque routeur en indiquant la destination, la passerelle (routeur suivant) et la distance (nombres de sauts) le séparant d’un autre routeur.
#. On relie un nouveau routeur E au routeur B. Donner la table de routage du routeur E et modifier les tables de routage des autres routeurs selon le protocole RIP.
#. Pour éviter l’isolement du routeur D, on le relie au nouveau routeur E. Corriger les tables de routage de chaque routeur.
#. On effectue des travaux sur le lien entre les routeurs C et D le rendant inopérant. Quelle sera alors la table de routage du routeur A selon le protocole RIP ?

Exercice 2
----------

On donne les tables de routage de 4 routeurs reliés dans un même réseau contenant 5 routeurs.

.. table:: **Routeur A**
   :align: center
   :class: border-on border-width-1

   +-----------+----------+--------+
   |Destination|Passerelle|Distance|
   +-----------+----------+--------+
   |     B     |    B     |   1    |
   +-----------+----------+--------+
   |     C     |    C     |   1    |
   +-----------+----------+--------+
   |     D     |    C     |   2    |
   +-----------+----------+--------+
   |     E     |    B     |   2    |
   +-----------+----------+--------+

.. table:: **Routeur B**
   :align: center
   :class: border-on border-width-1

   +-----------+----------+--------+
   |Destination|Passerelle|Distance|
   +-----------+----------+--------+
   |     A     |    A     |   1    |
   +-----------+----------+--------+
   |     C     |    A     |   2    |
   +-----------+----------+--------+
   |     D     |    E     |   2    |
   +-----------+----------+--------+
   |     E     |    E     |   1    |
   +-----------+----------+--------+

.. table:: **Routeur C**
   :align: center
   :class: border-on border-width-1

   +-----------+----------+--------+
   |Destination|Passerelle|Distance|
   +-----------+----------+--------+
   |     A     |    A     |   1    |
   +-----------+----------+--------+
   |     B     |    A     |   2    |
   +-----------+----------+--------+
   |     D     |    D     |   1    |
   +-----------+----------+--------+
   |     E     |    D     |   2    |
   +-----------+----------+--------+

.. table:: **Routeur D**
   :align: center
   :class: border-on border-width-1

   +-----------+----------+--------+
   |Destination|Passerelle|Distance|
   +-----------+----------+--------+
   |     A     |    C     |   2    |
   +-----------+----------+--------+
   |     B     |    E     |   2    |
   +-----------+----------+--------+
   |     C     |    C     |   1    |
   +-----------+----------+--------+
   |     E     |    E     |   1    |
   +-----------+----------+--------+

#. Le routeur A doit transmettre un message au routeur E en effectuant un minimum de sauts. Quel est le trajet parcouru ?
#. Donner une table de routage pour le routeur E.
#. Représenter par un graphe le réseau entre ces 5 routeurs.

Exercice 3
----------

Le protocole OSPF est utilisé dans un réseau.

#. Exprimer en bits par seconde, puis en Gb/s un débit de 50 Mb/s.
#. La liaison entre deux routeurs A et B a un débit de 100 Mbits/s. Calculer le coût de la liaison.
#. Le coût de la liaison entre deux routeurs A et C vaut 2. Calculer le débit entre ces deux routeurs.


Exercice 4
----------

On donne le graphe d’un réseau de 7 routeurs. Le protocole OSPF est utilisé entre ces routeurs pour communiquer.

.. figure:: ../img/graphe_reseau_3.png
   :align: center
   :width: 560

#. Reproduire le graphe en remplaçant chaque débit par son coût.
#. Déterminer le trajet qui a la plus faible coût entre les routeurs A et G. Justifier la réponse.
