# Guide de style

## Langue

La langue par défaut est le _français_.

L'utilisation d'accents est déconseillée dans les noms de fonctions et
diagrammes.

Eviter `get`, `set`, etc. et leur préférer un équivalent comme lire,
obtenir, récupérer, modifier, mettre à jour.

La veleur "`id` de `entitee`" se construit à la française: `idEntitee`.
Exemple: `idClient`

Omettre les articles (`le`, `la`), même pour les formes contractées comme `du`
(= `de le`). Exemple: `listerContactsClient` (au lieu de
`listerLesContactsDuClient`)

### Exemples

- `obtenirAgentParIdClient`

## Noms de fichier

`<code><id> - <titre>.<md|puml>`

### Codes

- CU: Cas d'Utilisation
- DSD: Diagramme de Séquence Détaillé
- DSS: Diagramme de Séquence Système
- ENT: Entité
- OM: Objet Métier
- SMA: Service Métier Applicatif (éviter l'abréviation `SM`)
- SOM: Service Objet Métier

### Id

A trois chiffres (ajouter des zéros à gauche si besoin).

Pas besoin de s'assurer que c'est continu, mais l'unicité doit être préservée.

## Style

### Casse

- Noms de fichiers: Casse mixte tolérée
  
  **ATTENTION AUX CHANGEMENTS DE CASSE**: Linux les supporte bien mais Windows
  peut être perdu.

- Entités: CapitalizedCamelCase

  **Exemple**: `Adresse`

- Attributs: camelCase

  **Exemple**: `clientId`
  
## Spécificités par type de document

### DSD



- Utiliser les noms `Interface` et `Services Métier Applicatifs`

- Les interactions etre `Agent` et `Interface` ne vont que dans le sens depuis
  l'agent vers l'interface.

- Pour les types de retour, séparer les clés étrangères de l'entité qui les
  utilise. Exemple: `getClientEtIdAgence(idClient)` retourne
  `Client, idAgence`.

- Mettre les arguments en gras (`**variable**`) et les retours en
  italique (`//variable//`)

- Noter les listes `Liste<var1, var2>`

- Pour les itérations, utiliser:

  ```puml
  group Pour chaque //idPersonne// de //Liste<idPersonne>//
      ...
  end
  ```
