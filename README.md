# Swisstopo IFC
Project to help improve the IFC format provided by Swisstopo



## Avis positif

1. L'accessibilité à l'IFC permet une démocratisation à la fois des données de Swisstopo et du format IFC

2. Identification simplifiée des objets (IfcBuildings, IfcWall/IfcRoof) : pratique pour certains usages (calcul des ombrages, etc.)

3. Plus de détail des toits en rapport au package de donnée swissBUILDINGS3D

<br>

## Amélioration souhaitée

1. Ajout des métadonnées pour rendre l'IFC exploitable
   (identification des bâtiments, zones, etc.)

2. Utile uniquement pour la géométrie (actuellement trop simplifiée): amélioration de la classification IFC des objets (murs, sols, toits)

3. Certains murs manquant sur l'IFC (donnée EPFL)

4. Géométrie proche du geopackage swissBUILDINGS3D avec les défauts de la structuration (Wall, Roof).
(Avec BlenderGIS, il est actuellement très facile d'importer une large zone de donnée via le format swissBUILDINGS3D).

5. Coordonnées des objets posant une impossibilité d'utiliser les données : les objets doivent être en relatif (point local 0,0,0) et avec un point de référence "global" avec les coordonnées nationales ou autre (EPSG:4326, EPSG 2056, etc.)

   Exemple : `#112=IfcCartesianPoint((2721558.704,1256990.225,564.623))`

    [voir «User Guide for Geo-referencing in IFC»](https://www.buildingsmart.org/standards/bsi-standards/standards-library/)

<br>
<br>

![blender-ifc.jpg](/images/blender-ifc.jpg)


## Idées complémentaires

1. Pouvoir un bâtiment pour faire une estimation d’une SIA380/1, pour un préprojet dans la rénovation avec toutes les limitations  :
    - Erreur de +/-30 cm qui peuvent donner 10% d’erreur sur la SRE
    - connaissance de combien le bâtiment est sous terre
    - connaissance de quelles parties sont chauffées ou pas
    - Les fenêtres et portes


## Remerciement

Merci pour les retour d'expérience à Raphaël V., Flavio F., Cyril W.