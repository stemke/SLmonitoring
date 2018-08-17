Un administrateur peut obtenir un point de vue holistique de la santé en cours et passée d'un périphérique à un seul endroit. 

Récits utilisateur :

    N'importe quel utilisateur peut basculer rapidement des onglets "Bande passante" et "Utilisation" de sa vue existante à ceux de l'application bêta Observer (bêta uniquement)

    N'importe quel utilisateur peut fournir des commentaires sur son expérience dans l'application bêta Observer via le portail de contrôle (bêta uniquement)

    N'importe quel utilisateur peut accéder à l'article de blogue pour en savoir plus à propos de notre travail dans Observer dans l'expérience bêta (bêta uniquement)

    Les utilisateurs disposent d'un lieu dédié dans lequel ils peuvent stocker et afficher les métriques de ressource d'infrastructure pour les serveurs virtuels :

    1. Utilisation de l'UC, %, par coeur virtuel

    2. Réseau public, octets et paquets, entrants/sortants

    3. Réseau privé, octets et paquets, entrants/sortants

    4. Utilisation de la mémoire, %

    5. Lecture disque, octets et opérations

    6. Ecriture disque, octets et opérations

    7. Erreurs de transmission, entrantes/sortantes, nombre

    8. Temps d'attente du disque, milliseconde, lecture et écriture

    9. Utilisation du disque local, % et octets utilisés et nombre total d'octets disponibles


    Les utilisateurs de périphérique bare metal pourront afficher les métriques suivantes :

    1. Utilisation de l'UC, %, par coeur virtuel

    2. Réseau public, octets et paquets, entrants/sortants

    3. Réseau privé, octets et paquets, entrants/sortants

    4. Utilisation de la mémoire, %

    5. Lecture disque, octets et opérations

    6. Ecriture disque, octets et opérations

    7. Erreurs de transmission, entrantes/sortantes, nombre

    8. Temps d'attente du disque, milliseconde, lecture et écriture

    9. Utilisation du disque local, % et octets utilisés et nombre total d'octets disponibles

    10. Alertes RAID, 0/1

    11. Température du coeur, degrés F

    N'importe quel administrateur peut afficher l'historique des alarmes et des métriques dans une seule vue sans avoir à analyser la consignation. (Semblable à #60.)

    Un gestionnaire peut comprendre la santé générale d'un périphérique sans avoir besoin d'une clarification de la part de ses équipes d'administration.

    N'importe quel utilisateur peut ouvrir le fichier syslog le plus récent d'un périphérique à l'aide de la ligne de commande. (Semblable à #35.)

    N'importe quel utilisateur peut afficher et explorer des données de métrique de série chronologique dans un ensemble de diagrammes interactifs. 

    N'importe quel utilisateur peut afficher et interpréter l'historique des alertes. 

    N'importe quel utilisateur peut marquer des événements comme "ouverts "ou "fermés". 

    Aucun utilisateur n'a besoin de créer manuellement un événement chaque fois qu'une alarme est déclenchée.

    Aucun utilisateur n'a besoin d'affecter manuellement un niveau de gravité "avertissement" ou "erreur" en plus de ses paramètres d'alarme.

    N'importe quel utilisateur peut rassembler des métriques de niveau système et application à l'aide d'agents collectD pour les processus de surveillance, Apache, Tomcat, MSSQL, MySQL et les réponses d'URL. 

    Un administrateur peut envoyer des données de métrique personnalisées dans le service de surveillance de façon automatisée.

    N'importe quel utilisateur peut employer des métriques système, application ou personnalisées de la même manière que des métriques d'hyperviseur : diagrammes, tableaux de bord, alarmes, notifications, réponses automatiques, modèles, etc. 



Cible métier 2 : un administrateur peut comprendre et commencer à identifier et résoudre un incident en 90 secondes

Récits utilisateur :

    N'importe quel administrateur peut s'abonner à des alertes sans être inondé de faux positifs.

    N'importe quel administrateur peut recevoir des alertes via son canal de communication de prédilection au cours de la minute que dure un événement déclencheur. 

    Les ingénieurs en fiabilité peuvent comprendre la cause d'une alerte d'incident en fonction du message contenu dans l'alerte proprement dite.

    N'importe quel administrateur peut rechercher des métriques d'utilisation récentes sur n'importe quel périphérique avec un haut degré de précision.

    N'importe quel administrateur peut trouver les informations exactes dont il a besoin en moins de 10 secondes.

    Un utilisateur non-administrateur peut résoudre un incident prioritaire avec moins de trois messages du support SL.

    N'importe quel utilisateur peut indiquer une condition visant à supprimer une alerte pour n'importe quelle métrique disponible (par défaut, collectD ou personnalisée).

    N'importe quel utilisateur peut indiquer une condition basée sur la valeur moyenne, cumulée (somme), minimale ou maximale de n'importe quelle métrique. 

    N'importe quel utilisateur peut indiquer une condition avec la qualification "supérieur à" ou "inférieur à". 

    N'importe quel utilisateur peut spécifier le nombre de périodes consécutives au cours desquelles une condition doit être réalisée, ainsi que la longueur de la période, 30 secondes ou 5 minutes, avant le déclenchement d'une alarme : "si X se produit au cours de 2 périodes consécutives de 30 secondes, une alarme se déclenche"

    N'importe quel utilisateur peut indiquer plusieurs conditions pour une seule alarme : "si ça ET ça ET ça, une alarme se déclenche"

    N'importe quel utilisateur peut indiquer un nom personnalisé pour l'alarme.

    N'importe quel utilisateur peut être informé des alertes indiquant l'heure, le nom de l'alarme, ainsi que les conditions ayant déclenché l'alarme.

    Aucun utilisateur, après le déclenchement d'une alarme, ne recevra d'alertes supplémentaires à partir de la même règle sur le même périphérique tant que l'alarme initiale n'aura pas été "fermée". 

    Exemple de règle d'alarme : si la moyenne d'utilisation de l'UC est supérieure à 80 % pour 2 périodes consécutives de 5 minutes ET la somme du trafic entrant sur le réseau est supérieure à 50 Go pour 1 période consécutive de 5 minutes, une alarme se déclenche et un événement est créé (si l'on part du principe que les éventuelles alarmes précédentes issues de cette règle ont été fermées). 

    Un administrateur peut spécifier une ou plusieurs adresses électroniques afin d'avertir des utilisateurs. 

    Un administrateur peut spécifier un ou plusieurs numéros de téléphone afin d'avertir des utilisateurs par SMS. 

    Un administrateur peut spécifier une ou plusieurs URL pour les webhooks à envoyer. 

    Un administrateur peut spécifier un groupe Pagerduty afin d'avertir des utilisateurs. 

    Un administrateur peut spécifier si le serveur doit redémarrer ou s'arrêter lorsque l'alerte est déclenchée.

    Un administrateur peut spécifier un intervalle de 30 secondes ou 5 minutes pour la surveillance réseau de n'importe quel protocole pris en charge. 

    Un administrateur peut implémenter des vérifications de ping d'hôte (ICMP).

    Un administrateur peut implémenter des vérifications de port TCP pour différents protocoles : DNS, DNS personnalisé, FTP, HTTP, HTTP personnalisé, HTTPS, IMAP, LDAP, NNTP, POP, SMTP, SSH, TCP personnalisé, TELNET, UDP SIP (la prise en charge pour ces protocoles existe dans l'offre SL TCP en cours). 

    Un administrateur peut implémenter une vérification de port TCP pour le protocole SNMP (non pris en charge actuellement dans l'offre SL existante).

    Un administrateur peut spécifier un seuil afin que le temps de réponse soit considéré comme une réussite ou une erreur. 

    Un administrateur peut spécifier le nombre d'erreurs consécutives générées par un ping d'hôte ou une vérification de port TCP avant le déclenchement d'une alarme. 

    Un administrateur peut implémenter les mêmes options de notification et de réponse automatisée à partir des alarmes de surveillance de réseau et à partir des alarmes basées sur des métriques (courrier électronique, SMS, webhook, PagerDuty, redémarrage, arrêt). 

    Un administrateur peut spécifier un niveau de gravité "avertissement" ou "erreur" pour les alarmes de surveillance de réseau et pour les alarmes basées sur des métriques.



Cible métier 3 : n'importe quel utilisateur peut configurer la surveillance sur n'importe quel périphérique en consacrant moins de 90 secondes à la prise de décisions concernant la configuration. (Semblable à #59.)

Récits utilisateur :

    Un utilisateur non-administrateur peut quasiment configurer sa surveillance en utilisant uniquement l'interface et la documentation.

    Un administrateur peut configurer une surveillance qui répond à ses besoins spécifiques en sélectionnant des configurations sauvegardées ou pré-conditionnées sans avoir à exécuter manuellement la configuration. (Semblable à #58.)

    Un administrateur peut configurer une surveillance qui répond à ses besoins spécifiques en éditant et en sauvegardant manuellement une configuration et en l'appliquant à n'importe quel nombre de périphériques. 

    Un administrateur peut configurer des alertes sur plusieurs périphériques avec un minimum d'efforts répétés.

    N'importe quel utilisateur peut exporter des données spécifiques au temps et aux métriques dans un fichier CSV. 

    Un administrateur ou un gestionnaire peut configurer une fenêtre de maintenance durant laquelle aucune notification n'est envoyée lorsque des alarmes sont déclenchées. 

    N'importe quel utilisateur expérimenté peut comprendre et appliquer des configurations sauvegardées. (Semblable à #41.)

    N'importe quel utilisateur débutant peut comprendre et appliquer des configurations pré-conditionnées. (Semblable à #34, #32.)

    Un utilisateur non-administrateur peut obtenir de l'aide pour configurer la surveillance sans avoir à remplir un ticket de demande de service. 

    N'importe quel client peut commander de la surveillance pour n'importe quel périphérique sans avoir des connaissances d'expert. (Semblable à #63, #43.)

    Tous les clients ont une expérience prévisible unifiée en matière de commande de surveillance pour n'importe quel périphérique. (Semblable à #40.)

    N'importe quel utilisateur peut intégrer son périphérique avec un service tiers sans avoir à remplir un ticket de demande de service. 

    Aucun utilisateur n'a besoin de créer manuellement une alarme pour le cycle de vie des alertes "avertissement" : création, démarrage, arrêt. 

    N'importe quel utilisateur technique peut accéder à toutes les fonctionnalités Observer via la même API que le reste du service de surveillance.

    IBM peut restreindre l'accès des comptes ab à certaines fonctions/performances avec une version gratuite, comme indiqué dans la présentation d'Observer pour le niveau gratuit par rapport au niveau payant. 

    N'importe quel client peut passer de la version gratuite à la version payante dans l'onglet Surveillance. 

    N'importe quel client peut effectuer une mise à niveau ou une rétromigration à partir des versions payantes ou gratuites dans la zone de gestion des comptes. 

    N'importe quel utilisateur possédant la version gratuite peut afficher les options dont il disposerait s'il avait effectué une mise à niveau, mais d'une manière qui indique la raison pour laquelle elles ne sont pas disponibles. 

    Si un utilisateur tente d'effectuer une action qui nécessiterait une mise à niveau, un message indiquant qu'il doit effectuer une mise à niveau et offrant une alternative, le cas échéant, s'affiche (par exemple, "Vous avez atteint le nombre maximal d'alarmes pour la version gratuite. Effectuez une mise à niveau ou supprimez une alarme pour créer une nouvelle règle.")


