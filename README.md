# Carte SEE ALL — donnees publiees

Ce depot ne sert qu'a une chose : heberger les GeoJSON que les calques distants
uMap vont lire. Une publication est un `git push` ; la carte se met a jour toute
seule au rechargement suivant.

## Calques

| Fichier | URL lue par uMap |
|---|---|
| `mc_a_faire.geojson` | https://raw.githubusercontent.com/michael-data-arch/seeall-carte/main/mc_a_faire.geojson |

Les calques de campagne MP s'ajoutent sous la forme `mp_<campagne>.geojson`.

## Regeneration

Depuis le depot `seeall-ops` :

```bash
scripts/publier.sh              # calque MC + campagnes actives
scripts/publier.sh --simulation # tout produire, ne rien ecrire ni pousser
```

`publish_map.sh` est hors service depuis la bascule du 22/08/2026 : il publiait
depuis liste_MC_SEEALL.xlsx, qui retardait sur Airtable et ne portait aucune fiche
d'acces.

## Ce depot est public

Les fiches d'acces y figurent en entier, codes de cadenas et telephones compris.
C'est un choix assume : le technicien doit trouver sur la carte de quoi ouvrir le
site sans ouvrir un second outil. Ne rien y ajouter qui n'ait pas ete decide.
