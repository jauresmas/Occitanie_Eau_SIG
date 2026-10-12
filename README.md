# Eau potable en Occitanie : lecture cartographique des pertes réseau par commune

Analyse en données ouvertes de la performance des services d'eau potable en Occitanie, croisant les indicateurs SISPEA avec le découpage communal de l'IGN.

## Ce que démontre le projet

- Chaîne complète en données ouvertes : récupération, nettoyage, jointure, analyse
- Base PostGIS (communes, indicateurs SISPEA, vue de jointure)
- Cartographie QGIS : rendement du réseau, volumes perdus, niveau de risque, opérateurs
- Carte web interactive autonome (Leaflet)

## Contenu

| Dossier | Rôle |
|---|---|
| `webmap/index.html` | Carte web interactive, données incluses dans le fichier |
| `exports/` | Cartes exportées depuis QGIS |

Les données volumineuses (GeoPackage, GeoJSON) ne sont pas versionnées. Elles se reconstituent à partir des sources ci-dessous.

## Sources

- SISPEA : indicateurs de performance des services d'eau et d'assainissement
- IGN Géoplateforme : limites communales ADMIN EXPRESS (service WFS)

Projection de travail : Lambert-93 (EPSG:2154).

Outils : QGIS, PostgreSQL / PostGIS, Leaflet.
