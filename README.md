# Cell Encounter Levels In Name

Trouve les niveaux minimum et maximum des zones et les ajoute aux noms des cellules en fonction du modèle spécifié. Les marqueurs de carte correspondants seront également modifiés pour refléter ces changements (ceci est désactivé de base).

## Fichier de configuration (Data/config.json)

- formulaRangedLeveled : Utilisé lorsque pour une zone le niveau maximum > au niveau minimum.
- formulaDeleveled : Utilisé lorsque les niveaux minimum et maximum d'une zone sont identiques.
- formulaLeveled : Utilisé lorsque le niveau minimum > au niveau maximum. Cela se produit généralement lorsque le niveau maximum n'est pas spécifié (0).
- patchMapMarkers : Indique si les marqueurs de carte doivent également être modifiés. (true/false).

## Fichier de configuration par défaut :
```
{
    "formulaRangedLeveled" : "{name} ({min} ~ {max})",
    "formulaDeleveled": "{name} ({min})",
    "formulaLeveled": "{name} ({min}+)",
    "patchMapMarkers": false
}
```
### Version à utiliser :
0.30.4 et 0.19.2
