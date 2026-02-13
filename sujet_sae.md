# Sujet de la SAE

## objectifs
L'objectif est de produire une analyse **en temps réel** de l'état de la menace internet et de s'en servir afin de renforcer la sécurité globale de vos serveurs et de vos postes clients et de l'application temps réel.
L'ensemble devra être opérationnel sur une période d'une semaine.


Tout d'abord vous devez mettre en place un pipeline de données depuis un honeypot TPOT.
L'honeypot devra être durci afin d'en limiter les accès :
- Access via Vpn
- Séparation des sondes de l'exploitation des données
- Authentification SSO
- Enregistrement des sessions de connexions, Bastion SSH
- Audit 
- Sauvegarde ...
- Supervision
- Rapports de sécurité à la demande et quotidien de votre infra.

Vous mettrez aussi en place une architecture virtualisée et containérisée en haute disponibilité avec de l'infra as code dont la sécurité sera amélioré par les résultats issus de vos honeypots.



L'analyse des logs sera faite en utilisant obligatoirement l'outil **polars** utilisé dans le language de développement de votre choix. Le mix des langage est permis.

la gestion du code suivra les bonnes pratiques (branche , tests, commit et merge réguliers...)
Les résultats temps réel seront aussi utilisés afin de protéger l'application d'analyse de la menace qui sera accessible depuis l'internet.

la gestion du code suivra les bonnes pratiques (branche , tests, commit et merge réguliers...)

### Organisation de la SAE

- Vous travaillerez en équipe de 6 personnes au minimum et de 7 personnes au maximum.   
- Vous travaillerez en mode agile (backlog, user story, sprint) et vous utiliserez un outil de gestion de projet pour gérer votre projet.
- Le reporting hebdomadaire personnalisé au niveau de chaque équipe est obligatoire précisant l'avancement du projet et la contribution de chacun.
Chaque tâche sera décrite avec ses caractéristiques (durée, intervenant, co-validateur..)
Au final un bilan des heures passées par tâche et par équipier sera réalisé.

Vous utiliserez gitlab.com comme serveur CI/CD. Chaque équipier devra participer au projet en utilisant des pull/merge requests pour chaque intégration sur une branche dev. 
Un coéquipier co-validera les MR/PR et les "mergera" avec la branche main. 



### Etapes de la SAE et livrables

- Vous écrirez un cahier des charges de l'application qui sera validé par le donneur d'ordre et rendu avant la phase de développement. Une maquette qui pourra être réalisée par IA est demandée.
- Vous écrirez un Cahier des charges Techniques des choix architecturaux qui devra être validé aussi. 
- Une application permettant de lister en temps réel l'état des menaces. Elle permettra de produire un rapport automatisé généré par IA et proposera un serveur MCP pour le faire avec récupération des informations en temps réel dans les logs.
- Un repository gitlab (mis à jour toutes les 8 heures) et  qui permettra de récupérer des listes noires et autres indicateurs de compromission. Des scripts prêt à l'emploie seront proposés pour des firewalls opensource. L'alimentation d'un serveur MISP serait apprécié. L'analyse des malwares collectés sera fortement apprécié.


- Vous utiliserez ces éléments afin de renforcer la protection périmétriques de votre parc de VM et votre clusters Kube ainsi qu'un serveur AD et de son client windows.
- La dernière semaine de la SAE sera celle de la mise en exploitation et vous devrez prouvez que l'application , l'alimentation des listes noires , ainsi que  la protection automatisée des postes seront fonctionnelles.
**Une soutenance finale sera réalisée pour présenter les résultats de votre travail et un rapport final est demandé.**

