# Dates en toutes lettres

Petit site qui convertit des dates en français écrit : `1/1/26` devient « premier janvier deux mille vingt-six ».

Tout fonctionne dans le navigateur, avec un seul fichier (`index.html`). Aucune dépendance, aucun serveur, aucune donnée envoyée.

## Utilisation

Saisissez une date par ligne (ou séparez-les par des points-virgules). Le résultat s’affiche en direct, avec un bouton pour copier chaque ligne ou tous les résultats.

| Saisie | Résultat |
|---|---|
| `1/1/26` | premier janvier deux mille vingt-six |
| `25-12-1999` | vingt-cinq décembre mille neuf cent quatre-vingt-dix-neuf |
| `25 août 1270` | vingt-cinq août mille deux cent soixante-dix |
| `1er mars` | premier mars |

### Formats reconnus

- Numériques : `1/1/26`, `01.01.2026`, `1-1-26`, `2026-01-01`, `01012026`, `010126`
- En toutes lettres : « 1er janvier 2026 », « jeudi 1 janv. 26 », « le 25 août 1270 »
- Sans année : `1/1`, « 14 mars », « 1er mars ». L’année est alors omise du résultat, et le jour de la semaine n’est pas affiché.

Les années vont de 1 à 9999. Les dates impossibles (31 février, 29 février d’une année non bissextile) sont signalées. Le 29 février sans année est accepté.

## Options

| Option | Choix |
|---|---|
| Ordre des dates numériques | jour/mois/année ou mois/jour/année |
| Années à 2 chiffres | seuil réglable : 20xx jusqu’à ce nombre, 19xx au-delà (50 par défaut) |
| Variante du français | France, Belgique (septante, nonante), Suisse romande (septante, huitante, nonante) |
| Orthographe | classique (vingt et un) ou rectifiée de 1990 (vingt-et-un, tirets partout) |
| Style des années | « mille deux cent soixante-dix » (défaut), « mil deux cent soixante-dix », « douze cent soixante-dix » |
| Présentation | « premier » ou « un », « le » en début, jour de la semaine, majuscule initiale, rappel de la date en chiffres |

Le thème clair ou sombre se change avec l’interrupteur en haut à droite. Par défaut, il suit le réglage de l’appareil, et le choix est mémorisé dans le navigateur.

## Limites

- Le jour de la semaine est calculé selon le calendrier grégorien appliqué rétroactivement. Pour une date antérieure à 1582, il peut différer de celui des sources historiques, qui suivent le calendrier julien.
- Les heures et les plages de dates (« du … au … ») ne sont pas gérées.

## Utiliser en local

Ouvrez simplement `index.html` dans un navigateur.