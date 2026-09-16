# SalonFinder — version 100% sans Google Maps API

Cette version utilise :
- OpenStreetMap pour la carte
- Overpass API pour chercher les `shop=hairdresser` et `shop=barber` à proximité
- la géolocalisation native du téléphone
- les données `opening_hours` d'OpenStreetMap pour déterminer le filtre ouvert/fermé
- OpenStreetMap/OSRM pour le bouton d'itinéraire

Aucune clé Google Maps n'est nécessaire.

## Limite importante : les avis

OpenStreetMap n'est pas un service d'avis clients. Il ne fournit pas les notes et avis Google. L'application affiche donc honnêtement qu'aucun système d'avis n'est disponible au lieu d'inventer des notes.

Si tu veux absolument les avis directement dans l'application, il faudra ajouter une source d'avis séparée disposant d'une API autorisée (par exemple un fournisseur d'avis avec quota gratuit), ce qui dépend de ses conditions et de sa couverture en France.

## Installation

Héberge le dossier en HTTPS, puis sur Android Chrome : menu → Ajouter à l'écran d'accueil / Installer l'application.

## Données et limites OSM

Les serveurs publics OpenStreetMap ont des limites et sont fournis sans garantie de disponibilité. Pour une application avec beaucoup d'utilisateurs, il est préférable d'utiliser un fournisseur OSM dédié ou sa propre infrastructure.

Attribution OSM obligatoire : © OpenStreetMap contributors.

Sources :
https://www.openstreetmap.org/copyright
https://operations.osmfoundation.org/policies/tiles/
https://operations.osmfoundation.org/policies/nominatim/
https://wiki.openstreetmap.org/wiki/Overpass_API
