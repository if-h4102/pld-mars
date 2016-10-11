# CU004 - Gestion des contrats du client (Zone Contrats)

L’agent voudra consulter la liste des contrats souscrits par le client dans
chaque domaine.

Un contrat a un code contrat, un intitulé, un descriptif, et un tarif de base.

Un contrat peut proposer des options (payantes ou gratuites), qui sont par
définition optionnelles et donc souscrites ou résiliées au fil du temps.

Selon les options choisies par le client, un tarif annuel est défini pour le
contrat souscrit (numéro de contrat, date de souscription).

Suite à la périodicité de paiement choisie par le client, une mensualité est
établie. 
L’origine de la souscription au contrat (date et agent) est mémorisée et
communiquée aux utilisateurs. 
Un client peut mettre fin à son contrat en le résiliant. 

**Etats de souscription à une option** : souscrite, non souscrite
