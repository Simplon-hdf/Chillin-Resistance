# Chillin-Resistance

# Stratégie de Sécurisation d'une application🔒

    Mesures visant à empêcher le vol ou le piratage des données.

************************************************************************************************************

# a \ Sauvegarde
     Nous avons utilisé la sauvegarde (backup en anglais) pour dupliquer et à mettre en sécurité les données contenues dans le base de donnée de la'application.

    Pour realiser l'objectif de la sauvegarde, nous avons utilisé la stratégie de sauvegarde la pluce efficace (La stratégie de sauvegarde 3-2-1).

# Nos sauvegardes grâce à la stratégie 3-2-1(3-2-1 backup rules):
     # La stratégie de sauvegarde 3-2-1 est composée de trois règles, elles sont les suivantes :

     * Trois copies de données - Cela inclut les données d'origine et au moins deux sauvegardes.

     * Deux types de stockage différents - Les deux copies des données sauvegardées doivent être conservées sur deux types de stockage distincts afin de minimiser les risques d'échec. Les types de stockage peuvent inclure un disque dur interne, un disque dur externe, un lecteur de stockage amovible ou un environnement de sauvegarde dans le cloud.t.

    * Une copie hors site - Au moins une copie de données doit être stockée dans un emplacement hors site ou distant pour garantir que les catastrophes naturelles ou géographiques ne peuvent pas affecter toutes les copies de données

# c\ Jornalisation
      Pour assurer la sécurité des traitements et la traçabilité des accès et des actions des utilisateurs , nous allons enregistrer dans des « fichiers journaux » ou (« logs ») des activités des utilisateurs, des anomalies et des événements liés à la sécurité. Obligation posée à l’article 5 du RGPD, fortement recommandé par CNIL(a Commission nationale de l’informatique et des libertés)


# d\ Audit: qu’est-ce que l'Audit ?
    Pour garder un oeil sur touts les utilisar de l'application, nous allons utiliser AUDIT de base de données, est un contrôle de sécurité de base de données impliquant plusieurs aspects de surveillance. Il permet aux administrateurs de contrôler l'accès, de savoir qui utilise la base de données et ce que les utilisateurs font avec la base de données.


# e\ Défense en profondeur:
    Pour assurer la securité de l'application, nous allons appliquer La défense en profondeur (DiD) est une approche de la cybersécurité dans laquelle une série de mécanismes défensifs sont superposés afin de protéger les données et informations précieuses. Si un mécanisme échoue, un autre intervient immédiatement pour contrecarrer une attaque

    # À quoi ressemble-t-il dans?

        - Endpoint security
        - wifif security
        - Database security
        - Browser security 
        - Email security
        - network access control 


# f\ Réduction de la surface d’attaque:

     Nous allons réduire la surface d'attaque est le nombre de tous les points possibles, ou vecteurs d'attaque, où un utilisateur non autorisé peut accéder à un système et extraire des données. Plus la surface d'attaque est petite, plus il est facile de protéger

     #La surface d'attaque est divisée en deux catégories :
      
         1\ Surface d'attaque numérique:
            La surface d'attaque numérique englobe tout le matériel et les logiciels qui se connectent au réseau d'une organisation. Il s'agit notamment des applications, du code, des ports, des serveurs et des sites Web ...

        2\Surface d'attaque physique:
            La surface d'attaque physique comprend tous les endpoint ou un attaquant peut obtenir un accès physique, comme  ordinateurs de bureau, disques durs, ordinateurs portables, téléphones mobiles et lecteurs Universal Serial Bus (USB)

# g\ Moindres priviliges:  qu’est-ce que la moindres priviliges ?
  Nous allons appliquer principe du moindre privilège (PoLP), qui fait référence à un concept de sécurité de l'information dans lequel un utilisateur reçoit les niveaux minimaux d'accès - ou d'autorisations - nécessaires.

 #Comment mettre en œuvre le moindre privilège?
    - Auditez l'environnement pour localiser les comptes privilégiés 
    - Éliminez les privilèges d'administrateur local inutiles et assurez-vous que tous les utilisateurs  disposent uniquement des privilèges nécessaires pour effectuer leur travail.

# h\ RBAC (Contrôle d’accès basé sur les rôles):
     Nous allons appliquer le concept Contrôle d’accès basé sur les rôles (RBAC), est un concept de sécurité du réseau selon lequel le réseau accorde des droits aux utilisateurs en fonction de leur rôle dans l’entreprise. 

     #RBAC : une mise en œuvre en 3 étapes:
        - Définissez les ressources et services que vous fournissez à vos utilisateurs .
        - Créez une bibliothèque de rôles : faites correspondre les descriptions de postes aux ressources définies à l’étape 1 nécessaires à la réalisation de leur mission
       -  Affectez les utilisateurs aux rôles définis.

# i\ RGPD (Le Règlement Général sur la Protection des Données):
Nous allons appliquer les Règlements (UE) 2016/679 du Parlement européen et du Conseil du 27 avril 2016, relatif à la protection des personnes physiques à l'égard du traitement des données à caractère personnel et à la libre circulation de ces données.


#RGPD : comment se mettre en conformité ?
#Il y a 4 étapes de mise en conformité à la loi RGPD.

Etape 1 : Constituer un registre des traitements (Journalisation)
    Ce registre vous permettra de recenser vos fichiers, tout en effectuant un suivi régulier de leur utilisation. Placé sous la responsabilité du dirigeant de l’entreprise, ce registre doit pouvoir être mis à jour régulièrement, avec l’aide des personnes chargées de la collecte des données.

    À noter que les PME de moins de 250 salariés ne sont pas dans l’obligation de tenir ce registre, bien que celles-ci soient concernées par la réglementation RGPD.

Etape 2 : Trier les données
    Ne prenez pas la mauvaise habitude d’accumuler. Vous récoltez des milliers de données, mais demandez-vous si ces dernières ont un réel intérêt pour le développement de votre activité. Ensuite, vérifiez que vous n’utilisez pas des données dites « sensibles » et si c’est le cas vérifiez que vous en avez le consentement (comme le prévoit la loi RGPD).

Etape 3 : Respecter le droit des personnes
     Depuis l’entrée en vigueur de la loi RGPD 2018, vous avez un devoir d’information et de transparences concernant la collecte et la transmission des données à caractère personnel.

    Pour ce faire, vous devez impérativement :

    - Expliquer la raison de cette collecte de données,

    - Demander le consentement de chaque utilisateur,

    - Indiquer qui aura accès à ces données et pour combien de temps, - Détailler les modalités selon lesquelles les personnes pourront exercer leurs droits d’effacement ou de modification par exemple,

    - Si ces données récoltées sont susceptibles de sortir de la zone européenne.

Etape 4 : Sécuriser les données
    Vérifiez que les données collectées soient suffisamment protégées des piratages et autres déconvenues informatiques. Changez régulièrement vos mots de passe, faites les mises à jour sur les antivirus, ne confiez pas l’accès des données à n’importe qui … Des choses simples qui sont malheureusement parfois négligées dans les petites entreprises. Le danger ne se mesurant pas au nombre de salariés, garder à l’esprit que ces données sensibles sont une mine d’or que beaucoup de personnes aimeraient s’approprie


# j\ Cookies
Nous allons utiliser les cookies pour avoir des informations sur les préférences de la personne qui visite le site, et aussi pour reconnaitre et conserver des informations, par exemple le choix de la langue, les identifiants de connexion, les pages consultées ou par exemple le contenu d’un panier, aussi pour obtenir des statistiques sur le site web en question 



************************************************************************************************************


