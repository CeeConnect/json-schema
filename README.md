# JSON Schema - Certificats d'économies d'énergie

Ce projet propose un vocabulaire uniformisé de référence au format YAML pour les acteurs du dispositif des Certificats d'Economies d'Energie (CEE), permettant la description, la validation et le partage de ressources.

## Structure du dictionnaire

**enums**: Regroupe les termes définis par un ensemble fermé de valeurs (eg une zone climatique n'accepte que trois constantes : H1, H2 et H3). Les énumérations peuvent être également sous-divisées par secteur d'application, un même terme pouvant avoir une définition différente selon le contexte.

**formats**: Regroupe les termes dont les valeurs doivent respecter une nomenclature (eg un numéro SIREN est une chaîne de neuf caractères numériques).

**mixins**: Regroupe les termes composés (eg une adresse est composée d'un numéro, d'une voie, d'un code postal...)

**bundles**: Regroupe les ressources métiers (eg un dépôt, un contrôle, une opération...)

## Guide

## Création d'une nouvelle fiche

1. Création du schéma d'opération
2. Création du schéma de simulation 
3. Création du schéma de contrôle

## Usages

- Validation de données JSON (JSON Schema)
- Génération automatique de formulaire HTML

## Spécification

- [JSON Schema](https://json-schema.org/) 2020-12

## Releases

### v0.3.0

- [x] Bâtiment résidentiel

### @next

- Couverture des contrôles

### @alpha-v2.0.0

- [x] Agriculture
- [x] Bâtiment résidentiel
- [x] Bâtiment tertiaire
- [x] Industrie
- [x] Réseau
- [x] Transport

## Doctrines

### Performances des équipements

Les performances et caractéristiques des équipements mentionnées par les fiches d'opérations standardisées couvertent par une réglementation nationale ou européenne ne sont pas validées. Elles sont considérées de facto cohérente avec le cadre réglementaire.

### Qualifications de l'installateur

Les schémas couvrent les contraintes de **qualifications RGE** requises pour le professionnel assurant la mise en oeuvre de l'opération.

**Les autres critères de qualifications (Qualibat ou équivalents) ne sont pas supportés pour le moment**.

###  BAR-EN-108v37-2

**L'attesation sur l'honneur prévoit la possibilité de renseigner plusieurs marques et référence dans le cas d'équipements installés de caractéristiques différentes, mais un unique champs relatif à la résistance thermique additionnelle.**

Afin de simplifier le dispositif, il est retenu qu'une fiche d'opération standardisée ne s'applique qu'à un ensemble cohérent d'équipements éligibles. Ainsi il conviendra de réaliser n dossiers avec n partie A de l'attestation sur l'honneur pour n équipements de caractéristiques différentes.
