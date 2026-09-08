# clinique_lfph

**Présentation de l'établissement**
LPFH Clinique est un établissement privé de santé implanté à Franceville depuis septembre 1981. Depuis mai
2021, elle fait partie du groupe VIVALTO, qui compte près de cinquante établissements en France.
La clinique emploie plus de 110 praticiens libéraux et 350 collaborateurs, qui assurent les consultations, les
interventions, les soins, l'hygiène et l'organisation des séjours.

C'est un établissement pluridisciplinaire : chirurgie viscérale, vasculaire, gynécologique et obstétrique,
dentaire, orthopédique, O.R.L., ophtalmologique, urologique, neurochirurgie, cancérologie, ainsi que des
spécialités médicales telles que cardiologie, gastro-entérologie, pneumologie, hématologie, neurologie,
endocrinologie, pédiatrie, réadaptation cardiaque, rééducation nutritionnelle et soins palliatifs.

Elle dispose également d'un service d'imagerie de radiologie, de cabinets de consultation, d'une maternité et
d'un centre AMP, d'un plateau technique d'accès direct en cardiologie et d'un service de soins non programmés
24h/24 — 7j/7. Elle accueille chaque année plus de 23 000 séjours dans 253 lits.

**1. La direction des systèmes d'information**
La DSI, installée dans les bâtiments de la clinique, est dirigée par Pierre LEMORT, responsable sécurité des
systèmes d'information. Elle est organisée en trois pôles de compétences :
- Le pôle « Infrastructures et serveurs » a pour activités principales le paramétrage et la sécurisation des
éléments d'interconnexion des serveurs.
- Le pôle « Applications » est dédié au développement d'applications spécifiques et à la maintenance
des applications pour les besoins de la clinique.
- Le pôle « Données à caractère personnel et données sensibles » (RGPD) a pour mission de veiller à
l'identification des risques et au respect de la législation sur les données à caractère personnel.

La clinique assure le filtrage entre les différents services par le firewall. Les services « Libéraux », «
Laboratoire », « Joliot Curie », « Biomédical » et « Radiologie » envoient et reçoivent des données depuis les
serveurs gérant le dossier administratif et médical du patient du service « LPF Clinique ». La plupart des
services disposent par ailleurs d'un accès Internet indépendant.

**2. Organisation du système d'information de la clinique**
On trouve de nombreuses applications métier (base d'information patients, serveurs dédiés à la recherche, base
de données des produits de la pharmacie, base de données des licences d'exploitation logicielles, etc.) ainsi
que les fonctions plus génériques de toute entreprise (Progiciel de Gestion Intégré avec ses modules RH,
GRC, etc.).

Un nombre croissant de serveurs est virtualisé. Constitué autour de VLAN, le réseau segmente les services de
manière à fluidifier le trafic.

Les données de l'entreprise sont considérées comme stratégiques et ne peuvent tolérer ni fuite, ni destruction :
l'ensemble des informations est répliqué quotidiennement dans le VLAN dédié BACKUP par un lien dédié.
Toutes les fonctions de redondance (RAID, alimentation, lien réseau redondant, Spanning-tree, clustering,
etc.) sont mises en œuvre pour assurer une tolérance aux pannes maximale.
Libertés et contraintes laissées à chaque clinique du groupe
- Chaque clinique du groupe VIVALTO est libre de ses choix matériels et logiciels concernant ses
serveurs.
- Chaque clinique est libre de regrouper ou non plusieurs services sur une même machine.
- Aucun système d'exploitation n'est imposé au niveau du groupe : chaque clinique choisit librement le
ou les systèmes d'exploitation, pour ses serveurs comme pour ses postes clients.
- Chaque clinique est libre dans l'organisation de ses VLAN ou réseaux ; seule obligation : les serveurs
doivent être isolés dans un VLAN ou un réseau spécifique. Selon les secteurs, les postes patients
peuvent être répartis sur plusieurs VLAN.
 Dans chaque clinique existe un réseau de test isolé du réseau du site, destiné au développement des
applications.
