# Chillin-Resistance

Pour cette application , nous avons été confronté à différentes problèmatiques concernant la sécurité. Nous avons mis en oeuvre un process détaillé pour chaque grande partie importante que nous allons décrire ci-dessous.

# Stratégie de Sécurisation d'une application🔒

   Mesures visant à empêcher le vol ou le piratage des données.

************************************************************************************************************

## a \ Sauvegarde
Nous avons utilisé la sauvegaSimon-Libert/Chillin-Resistancerde (backup en anglais) pour dupliquer et à mettre en sécurité les données contenues dans le base de donnée de la'application.

Pour realiser l'objectif de la sauvegarde, nous avons utilisé la stratégie de sauvegarde la pluce efficace (La stratégie de sauvegarde 3-2-1).

## Nos sauvegardes grâce à la stratégie 3-2-1(3-2-1 backup rules):
   # La stratégie de sauvegarde 3-2-1 est composée de trois règles, elles sont les suivantes :

   * Trois copies de données - Cela inclut les données d'origine et au moins deux sauvegardes.

   * Deux types de stockage différents - Les deux copies des données sauvegardées doivent être conservées sur deux types de stockage distincts afin de minimiser les risques d'échec. Les types de stockage peuvent inclure un disque dur interne, un disque dur externe, un lecteur de stockage amovible ou un environnement de sauvegarde dans le cloud.t.

   * Une copie hors site - Au moins une copie de données doit être stockée dans un emplacement hors site ou distant pour garantir que les catastrophes naturelles ou géographiques ne peuvent pas affecter toutes les copies de données

## c\ Jornalisation
   Pour assurer la sécurité des traitements et la traçabilité des accès et des actions des utilisateurs , nous allons enregistrer dans des « fichiers journaux » ou (« logs ») des activités des utilisateurs, des anomalies et des événements liés à la sécurité. Obligation posée à l’article 5 du RGPD, fortement recommandé par CNIL(a Commission nationale de l’informatique et des libertés)


## d\ Audit: qu’est-ce que l'Audit(PASSI) ?
Un audit de cybersécurité est un audit qui vise à améliorer le niveau de sécurité des systèmes d’information. Cela va des tests d’intrusion aux tests de configuration, aux audits d’architecture et aux audits de la politique de sécurité des entreprises. Pour garantir la bonne réalisation de ces audits, il est fortement recommandé d’avoir recours à un prestataire qualifié PASSI par l’Agence nationale de la sécurité des systèmes d’information (ANSSI).

pourquoi audit(PASSI):

•    D’évaluer le niveau de sécurité de votre système d’information
•    De déterminer les écarts par rapport aux normes
•    De détecter d’éventuelles failles de sécurité

Elles peuvent porter sur cinq domaines :

Tests d’intrusion
    Le principe du test d’intrusion est de découvrir des vulnérabilités sur le système d’information et de vérifier leur exploitabilité et leur impact, dans les conditions réelles d’une attaque, à la place d’un attaquant potentiel.

Audit d’architecture
    Il consiste en la vérification de la conformité des dispositifs matériels et logiciels. Il est efficacement accompagné de tests d’intrusion mais peut être réalisé seul.

Audit de configuration
    Il s’agit pour l’auditeur de vérifier conformément à l’état de l’art ou aux exigences et règles spécifiques de l’auditer, la sécurité des configurations de vos équipements et serveurs. Cet audit est efficacement accompagné de tests d’intrusion mais peut être réalisé seul.

Audit de code source
    Il s’agit d’analyser le code de vos applications afin de détecter d’éventuelles faiblesses. L’audit de code source doit permettre d’éviter les fuites d’information et les altérations du fonctionnement du système d’information.

## e\ Défense en profondeur:
   Pour assurer la securité de l'application, nous allons appliquer La défense en profondeur (DiD) est une approche de la cybersécurité dans laquelle une série de mécanismes défensifs sont superposés afin de protéger les données et informations précieuses. Si un mécanisme échoue, un autre intervient immédiatement pour contrecarrer une attaque

   ## À quoi ressemble-t-il dans?

   - Endpoint security
   - wifif security
   - Database security
   - Browser security 
   - Email security
   - network access control 


## f\ Réduction de la surface d’attaque:

   Nous allons réduire la surface d'attaque est le nombre de tous les points possibles, ou vecteurs d'attaque, où un utilisateur non autorisé peut accéder à un système et extraire des données. Plus la surface d'attaque est petite, plus il est facile de protéger

   ##La surface d'attaque est divisée en deux catégories :
      
  1\ Surface d'attaque numérique:
            La surface d'attaque numérique englobe tout le matériel et les logiciels qui se connectent au réseau d'une organisation. Il s'agit notamment des applications, du code, des ports, des serveurs et des sites Web ...

   2\Surface d'attaque physique:
            La surface d'attaque physique comprend tous les endpoint ou un attaquant peut obtenir un accès physique, comme  ordinateurs de bureau, disques durs, ordinateurs portables, téléphones mobiles et lecteurs Universal Serial Bus (USB)

## g\ Moindres priviliges:  qu’est-ce que la moindres priviliges ?
  Nous allons appliquer principe du moindre privilège (PoLP), qui fait référence à un concept de sécurité de l'information dans lequel un utilisateur reçoit les niveaux minimaux d'accès - ou d'autorisations - nécessaires.

 #Comment mettre en œuvre le moindre privilège?
    - Auditez l'environnement pour localiser les comptes privilégiés 
    - Éliminez les privilèges d'administrateur local inutiles et assurez-vous que tous les utilisateurs  disposent uniquement des privilèges nécessaires pour effectuer leur travail.

## h\ RBAC (Contrôle d’accès basé sur les rôles):
   Nous allons appliquer le concept Contrôle d’accès basé sur les rôles (RBAC), est un concept de sécurité du réseau selon lequel le réseau accorde des droits aux utilisateurs en fonction de leur rôle dans l’entreprise. 

   ## RBAC : une mise en œuvre en 3 étapes:
        - Définissez les ressources et services que vous fournissez à vos utilisateurs .
        - Créez une bibliothèque de rôles : faites correspondre les descriptions de postes aux ressources définies à l’étape 1 nécessaires à la réalisation de leur mission
       -  Affectez les utilisateurs aux rôles définis.

## i\ RGPD (Le Règlement Général sur la Protection des Données):
Nous allons appliquer les Règlements (UE) 2016/679 du Parlement européen et du Conseil du 27 avril 2016, relatif à la protection des personnes physiques à l'égard du traitement des données à caractère personnel et à la libre circulation de ces données.


##RGPD : comment se mettre en conformité ?
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


## j\ Cookies
Nous allons utiliser les cookies pour avoir des informations sur les préférences de la personne qui visite le site, et aussi pour reconnaitre et conserver des informations, par exemple le choix de la langue, les identifiants de connexion, les pages consultées ou par exemple le contenu d’un panier, aussi pour obtenir des statistiques sur le site web en question 



************************************************************************************************************

## Les requêtes et la sécurisation de l'API

En ce qui concerne les requêtes http, nous allons mettre en place un système de sécurisation qui va permettre d'éviter certaines attaques cibles, compte tenu du fait que le client va en permanence faire des requêtes vers nos APIs (application programming interface que l'on va créer afin d'appeler à la demande du client - lors du visionnage d'une vidéo - les vidéos stockées)lors des visionnages des différents cours proposés : 

- Cela commence par la configuration des **CORS** (Cross-origin resource sharing
 ou partage des ressources entre origines multiples) : 
 C'est un mécanisme qui consiste à ajouter des en-têtes HTTP afin de permettre à 
un agent utilisateur d'accéder à des ressources d'un serveur situé sur 
une autre origine que le site courant. Un agent utilisateur réalise une 
requête HTTP **multi-origine (*cross-origin*)** lorsqu'il demande une ressource provenant d'un domaine, d'un protocole ou d'un port différent de ceux utilisés pour la page courante.

Le CORS permet de prendre en charge des requêtes multi-origines 
sécurisées et des transferts de données entre des navigateurs et des 
serveurs web. Les navigateurs récents utilisent le CORS dans une API 
contenante comme `[XMLHttpRequest](https://developer.mozilla.org/fr/docs/Web/API/XMLHttpRequest)`
 ou `[Fetch](https://developer.mozilla.org/fr/docs/Web/API/Fetch_API)`
 pour aider à réduire les risques de requêtes HTTP multi-origines.

- exemple de requête fetch vers une api : 

```
export const getEventById = async (id, token) => {
  const res = await fetch(
    `${process.env.NEXT_PUBLIC_API_URL}/events/${id}`,
    {
      method: 'GET',
      headers: {
        'Content-Type': 'application/json',
        Authorization: 'Bearer ' + token
      }
    }
  )
  const data = await res.json()
  return data.event}

```

On remarque que lors de notre requête nous configuronsle type de content, ainsi que le passage d'un token (une clef chiffrée) afin de sécurisé l'appel API. Puis une réponse est attendue.

On met également en place les SOP : same origin policy. Nous vérifions que deux pages ont la même origine si le protocole - HTTP -, le port (si spécifié) et l'hôte - store.company -sont les mêmes pour les deux pages. Le tableau suivant présente des comparaisons d'origines pour l'URL

exemple : 

| http://store.company.com/dir2/other.html | Succès |  |
| --- | --- | --- |
| http://store.company.com/dir/inner/another.html | Succès |  |
| https://store.company.com/secure.html | Échec | Protocoles différents |
| http://store.company.com:81/dir/etc.html | Échec | Ports différents |
| http://news.company.com/dir/other.html | Échec | Hôtes différents |

La mise en place de requête HTTP permet aussi d'élaborer une stratégie de sécurisation de contenu : le CSP que l'on place dans l'entête de la requête - dans le HEADER -.

**D'ailleurs la mise en place d'un CSP permet également de réduire l'impact des requêtes silencieuses via CSP** - voir [requêtes silencieuses][] -

Aujourd'hui la norme pour les requêtes HTTP est l'ajout du **HSTS** qui fait la transmission d’un en-tête HTTP lors de l’accès au site en HTTPS pour assurer son intégrité.

Il est obligatoire de posséder le protocole **HTTPS** afin de garantir la sécurité des données et de l'utilisation de l'application à l'utilisateur. La mise en place de HTTPS a pour objectif :
■ de garantir, autant que possible, l’authenticité du site consulté ;
■ de garantir également l’intégrité et la confidentialité des données échangées en bloquant les
attaques de type Man-In-The-Middle (écoute, interception ou modification des échanges à la
volée par des tiers, à l’insu de l’utilisateur).

Nous utiliserons également le protocole TLS, un protocole important de communication sur les réseaux et internet. Il permet une communication chiffrée entre un client et un serveur. Les données applicatives sont encapsulées de manière à assurer la confidentialité et l’intégrité des échanges. Le serveur est nécessairement authentifié, et des fonctions additionnelles permettent l’authentification du client lorsqu’un tel besoin a été identifié.C’est un protocole en poignée de main (Handshake) car le client et le serveur **négocie la connexion TLS**.
TLS est utilisé pour la connexion des sites HTTPS. Mais depuis, on trouve des déclinaisons par exemple avec les protocoles POP ou SMTP pour les serveurs mails (MTA).

**Sécurisation d’API :**

Les fonctionnalités des API Web sont soumises aux mêmes 
considérations de sécurité que JavaScript et les autres technologies web
 (par exemple [same-origin policy](https://developer.mozilla.org/fr/docs/Web/Security/Same-origin_policy)),
 mais elles disposent parfois de mécanismes de sécurité supplémentaires.
 Par exemple, certaines des API Web les plus modernes ne fonctionneront 
que sur des pages servies par HTTPS, car elles transmettent des données 
potentiellement sensibles (par exemple [Service Workers](https://developer.mozilla.org/fr/docs/Web/API/Service_Worker_API) et [Push](https://developer.mozilla.org/fr/docs/Web/API/Push_API)).

En outre, certaines API Web demandent la permission d'être activées à
 l'utilisateur une fois que les appels à ces interfaces sont effectués 
dans votre code. À titre d'exemple, l'API [Notifications API](https://developer.mozilla.org/fr/docs/Web/API/Notifications_API) demande la permission à l'aide d'une boîte de dialogue contextuelle :

![https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Introduction/notification-permission.png](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Introduction/notification-permission.png)

Les API Web Audio et `[HTMLMediaElement](https://developer.mozilla.org/fr/docs/Web/API/HTMLMediaElement)`
 sont soumises à un mécanisme de sécurité appelé [autoplay policy (en-US)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API/Best_practices)

 - cela signifie essentiellement que vous ne pouvez pas lire 
automatiquement l'audio lorsqu'une page se charge — vous devez permettre
 à vos utilisateurs de déclencher la lecture audio par le biais d'un 
contrôle comme un bouton. Cette mesure est prise parce que la lecture 
automatique de l'audio est généralement très ennuyeuse et que nous ne 
devrions pas y soumettre nos utilisateurs.

Dans le cadre de notre application, nous allons devoir demander au user de bien vouloir accepter d'authoriser l'application à lui envoyer des notifications. 

**Requêtes silencieuses**

Certaines fonctionnalités de la spécification HTML permettent de demander au navigateur d’émettre des requêtes silencieuses sans passer par l’exécution de code
JavaScript ou CSS. Comme tout comportement qui conduit le navigateur
d’une victime à initier une connexion de manière silencieuse, ces
requêtes sont potentiellement indésirables et présentent des
risques allant de la fuite d’informations jusqu’à l’exploitation
de failles CSRF en passant par la réalisation d’attaques par déni
de service distribué (DDoS).

Exemple : 
Ce genre de fonctionnalité est l’attribut ping. Une balise HTML peut, si
celle-ci présente un attribut href, comporter un attribut ping en
complément. L’attribut ping contient alors une liste d’URLs vers
lesquelles seront réalisées des requêtes POST lorsque le lien sera
cliqué. Les URLs définies par l’attribut ping peuvent se situer
en dehors de l’Origin et son utilisation relève généralement du
tracking publicitaire.

**Sanitization** : 
C'est l’action de nettoyer, dans le sens ou elle permet de mettre en
place un filtre afin de traiter les informations reçues et
voir si elle correspondent plus au moins au résultat attendu.

Exemple :
Dans le cas d’un formulaire d’inscription, la sanitization
met un filtre afin de vérifier que dans le champs email, il s’agit
bel et bien d’un email entré dans le champ.


## Politique de sécurité des mots de passe

### R-20 Mettre en place une politique de sécurité des mots de passe

Les mots de passe présentent de nombreuses limites à la fois du point de vue de leur utilisation et de leur gestion.

On peut distinguer trois catégories de mots de passe :
- Les mots de passe devant être mémorisés:
Mot de passe maître d’un coffre-fort de mots de passe, d’une session Windows, etc. 
Ces mots de passe doivent être mémorisés et suffisamment robustes au vu de leur criticité, mais ils sont peu nombreux à retenir. Cette catégorie de mot de passe étant la plus critique, il est pertinent qu’elle soit associée à un second facteur d’authentification.
- Les mots de passe pouvant ne pas être mémorisés :
Concerne les mots de passe pouvant être générés et conservés par des coffres-forts de mots de passe, comme les mots de passe associés à des comptes de récupération.
- Les numéros d’identification personnels, (codes PIN) qui sont vérifiés localement au sein d’un composant physique de sécurité. Généralement accompagnés de mesures très restrictives sur le nombre d’échecs d’authentification autorisés.


**Longueur des mots de passe**

La robustesse d’un mot de passe est généralement mesurée au moyen de l’entropie, exprimée en bits. L’entropie d’un mot de passe peut être estimée en calculant l’ensemble des mots de passe possibles pour une longueur donnée et une complexité donnée. 
Il est souvent plus efficace d’allonger un mot de passe que de chercher à le rendre plus complexe pour en augmenter l’entropie. 
Définir une longueur minimale permet d’avoir un certain contrôle sur le niveau de sécurité apporté par les mots de passe lors de leur création par les utilisateurs.

### R21 - Imposer une longueur minimale pour les mots de passe

Il est recommandé de définir une longueur minimale pour les mots de passe lors de leur création en fonction du niveau de sécurité visé par le système d’information

### R22 - Ne pas imposer de longueur maximale pour les mots de passe

Selon les systèmes, il est recommandé de ne pas fixer de limite à la longueur maximale d’un mot de passe afin de permettre aux utilisateurs d’avoir recours à des phrases de passe ou longs mots de passe.

En pratique selon les systèmes utilisés il paraît néanmoins raisonnable de fixer une valeur limite (plusieurs centaines de caractères par exemple) afin de ne pas s’exposer à de potentielles attaques en déni de service.

### R23 - Mettre en œuvre des règles sur la complexité des mots de passe

Au moment de la création ou du renouvellement d’un mot de passe par un utilisateur, il est re-commandé de mettre en œuvre des règles de complexité tout en proposant un jeu de caractères le plus large possible.

### R24 - Ne pas imposer par défaut de délai d'expiration sur les mots de passe des comptes non sensibles

Si la politique de mots de passe exige des mots de passe robustes et que les systèmes permettent son implémentation, alors il est recommandé de ne pas imposer par défaut de délai d’expiration sur les mots de passe des comptes non sensibles comme les comptes utilisateur

### R25 - Imposer un délai d'expiration sur les mots de passe des comptes à privilèges

Il est recommandé d’imposer un délai d’expiration sur les mots de passe des comptes très sen-sibles comme les comptes administrateurs. Ce délai d’expiration peut par exemple être fixé à une durée comprise entre 1 et 3 ans.

### R26 - Révoquer immédiatement les mots de passe en cas de compromission suspectée ou avérée

En cas de compromission suspectée ou avérée d’un système d’authentification, tous les mots de passe concernés par ce système doivent être renouvelés immédiatement (de l’ordre de la jour-née). Au-delà de ce délai, les comptes concernés doivent être désactivés et une procédure de ré-activation pour les utilisateurs doit être mise en œuvre.

Contrôle de la robustesse des mots de passe

### R27 - Mettre en place un contrôle de la robustesse des mots de passe lors de leur création ou de leur renouvellement

Il est recommandé de procéder à un contrôle automatisé et systématique de la robustesse des mots de passe au moment de leur création ou de leur renouvellement.

De nombreux contrôles permettent de s’assurer que les mots de passe ainsi créés offrent une ro-bustesse en accord avec le niveau de sécurité souhaité, par exemple :

- vérifier que les mots de passe respectent bien les règles définies dans la politique de sécurité des mots de passe ; 
- comparer les mots de passe lors de leur création à des mots de passe les plus utilisés ou bien ceux qui ont été compromis ; 
- repérer les mots de passe contenant des motifs (ou des répétitions) spécifiques ( « 12345 »« azerty », etc); 
- repérer les mots de passe contenants des informations personnelles, comme les noms et pré-noms ou encore les dates de naissance; 
- lors d’un renouvellement du mot de passe, interdire la réutilisation d’un mot de passe parmi les X derniers mots de passe déjà utilisés.


**Stockage des mots de passe**

Le stockage des mots de passe des utilisateurs doit être réalisé de manière sécurisée.

En cas de compromission de cette base, les mots de passe seront directement révélés s’ils sont stockés en clair. Ainsi, ce sont les empreintes des mots de passe qu’il faut conserver plutôt que les mots de passe eux-mêmes. 

Le stockage des mots de passe en clair doit être absolument proscrit. Ces empreintes, aussi appelées hachés, sont le résultat d’une fonction de hachage cryptographique (comme les familles SHA2 (Secure Hash Algorithm) ou SHA3) appliquée aux mots de passe.
Les fonctions de hachage cryptographique qui permettent de calculer ces empreintes sont déter-ministes. Autrement dit, l’empreinte d’un même mot de passe calculée avec la même fonction de hachage sera toujours la même. 

Il peut être alors possible de précalculer des tables de correspondance entre les mots de passe courants et leurs empreintes respectives pour différentes fonctions de hachage, ce qui accélère fortement le « cassage » des mots de passe. L’ajout d’une valeur aléatoire unique (communément appelée un sel) lors du calcul de l’empreinte du mot de passe permet de se prémunir contre des attaquants utilisant des tables précalculées.

### R28 - Utiliser un sel aléatoire long

Les fonctions de hachage cryptographique recommandées, comme la famille SHA2, sont des fonc-tions très rapides à exécuter, ce qui, dans le contexte du stockage des mots de passe, est un avan-tage pour les attaquants. Il est recommandé d’utiliser des fonctions de dérivation de mots de passe dites memory-hard permettant à la fois d’augmenter le temps d’exécution mais aussi l’espace mémoire lors du calcul d’une empreinte. L’utilisation de telles fonctions correctement paramétrées permet un important ralentissement des attaques par force brute tout en ayant un impact négli-geable sur les services légitimes ne devant exécuter qu’un petit nombre de calculs d’empreintes. 


**Recouvrement d'un accès**


### R30 - Proposer une méthode de recouvrement d'accès

Afin de permettre aux utilisateurs de retrouver un accès à leur compte, il est recommandé de mettre en place une méthode de recouvrement d’accès adaptée au contexte d’utilisation.

### R31 - Mettre à disposition un coffre-fort de mots de passe

Il est recommandé que les responsables du système d’information mettent à disposition des utili-sateurs un coffre-fort de mots de passe et les forment à son utilisation.


**Recommandations à destination des utilisateurs**

### R32 - Utiliser des mots de passe robustes

### R33 - Utiliser un mot de passe différent pour chaque service

### R34 - Utiliser un coffre-fort de mots de passe

### R35 - Protéger ses mots de passe

### R36 - Utiliser un mot de passe robuste pour l'accès à sa messagerie électronique

### R37 - Choisir un mot de passe sans information personnelle

### R38 - Modifier les mots de passe par défaut


## Authentification et Authorisation

 « L’identification est l’action consistant à identifier un objet ou un individu. »
« L’authentification est un processus permettant au système de s’assurer de la légitimité de la demande d’accès faite par une entité […] afin d’autoriser l’accès de cette entité à des ressources du système. » Par exemple, en comparant le mot de passe saisi avec celui stocké dans la base de données.
« L’autorisation est la fonction spécifiant les droits d’accès vers les ressources. »

## Sécurisation de l’authentification

**Authentification multifacteurs:**

L’authentification multifacteur découle de la nécessité de renforcer la sécurité apportée par l’utilisation d’un unique facteur d’authentification, particulièrement lorsqu’il s’agit d’un mot de passe utilisé seul. Ainsi même si ce dernier est compromis, un facteur supplémentaire d’un type différent est requis afin de s’authentifier.

Un facteur d’authentification est donc un facteur lié à une personne, relevant de diverses catégories :

**Facteur de connaissance:**
« ce que je sais », il s’agit d’une connaissance devant être mémorisée telle qu’une phrase de passe, un mot de passe, un code etc...

**Facteur de possession:**
« ce que je possède », il s’agit d’un élément secret non mémorisable contenu dans un objet physique qui idéalement protège cet élément de toute extraction, tel qu’une carte à puce, un token, un téléphone etc...

**Facteur inhérent:**
« ce que je suis », il s’agit d’une caractéristique physique intrinsèquement liée à une personne et indissociable de la personne elle-même, telle qu’une caractéristique biologique (ADN), morphologique (empreinte digitale, empreinte rétinienne) ou comportementale (voix, frappe au clavier).

La principale menace contre laquelle l’authentification cherche à se protéger est l’usurpation d’identité, qui consiste pour un attaquant à se faire passer pour un utilisateur légitime auprès du vérifieur.

Il est possible de distinguer deux grands types d’attaquants.
- Attaquant en ligne : l’attaquant peut uniquement interagir avec le serveur d’authentification pour tenter de retrouver une valeur secrète (un mot de passe ou une clé privée par exemple).
Il doit par exemple être capable d’interagir avec un serveur Web afin de réaliser son attaque. Se protéger contre des attaquants en ligne nécessite de mettre en place des mesures spécifiques,
comme le blocage temporaire de l’accès au compte pendant plusieurs secondes, voire minutes,
après un certain nombre d’essais infructueux.
- Attaquant hors ligne : l’attaquant peut interagir avec le serveur d’authentification, et a également accès aux données permettant au vérifieur de contrôler l’identité du prouveur (par
exemple des empreintes de mots de passe ou une clé publique). L’attaquant n’a pas besoin d’interagir avec le serveur pour réaliser son attaque et a alors accès à une puissance de calcul potentiellement très importante.

Se protéger contre des attaquants hors ligne nécessite que le vérifieur protège correctement les données permettant de contrôler l’identité des utilisateurs lors de l’authentification, par exemple en utilisant des fonctions de hachage dédiées pour le stockage des mots de passe ou en utilisant des protocoles d’authentification considérés comme forts.

De nombreux types d’attaques peuvent être menés contre un protocole d’authentification pour parvenir à usurper une identité. Nous pouvons citer :

- Les attaques par force brute : tests automatisés de tous les mots de passe et de toutes les clés cryptographiques possibles.

- Les attaques sur le protocole d’authentification : attaques de l’homme-du-milieu, attaques par rejeu, exploitation de vulnérabilité de l’implémentation etc...

- Le vol du moyen d’authentification : vol d’une carte à puce, récupération d’un mot de passe par hameçonnage, manipulation par l’ingénierie sociale, etc...

Certains protocoles d’authentification prennent en compte ces différentes attaques alors que d’autres méthodes nécessitent des mesures complémentaires afin d’en atténuer les conséquences.

### Facteurs de connaissance:

Les principales menaces pesant sur les facteurs de connaissance sont la déduction (au moyen d’attaques par recherche exhaustive ou par dictionnaire par exemple), l’hameçonnage, l’écoute (dans
le cas où l’envoi du facteur de connaissance est effectué au travers d’un canal non protégé), etc...

Les mots de passe, souvent choisis par les utilisateurs, font ainsi face à des attaques spécifiques :

- Attaque par recherche exhaustive. Cette attaque consiste à choisir un ensemble de caractères et à tester automatiquement toutes les combinaisons possibles de ces caractères. Une variante
de cette attaque, désignée par l’expression anglaise password spraying, consiste à effectuer des tests automatisés d’un nombre réduit de mots de passe (par exemple à partir d’une liste de
mots de passe très utilisés) mais pour un grand nombre d’identifiants possibles (ou de comptes de différents service web par exemple).

- Attaque par dictionnaire. Cette attaque consiste à faire l’hypothèse que le mot de passe recherché est un mot du dictionnaire d’une langue donnée et à tester automatiquement chacun de ces mots. Des dictionnaires plus aboutis intègrent également des variations courantes sur les mots du dictionnaire (transformation de a en @ par exemple), une liste des mots de passe ou des phrases de passe les plus utilisés ou bien encore une combinaison (concaténation, etc.) de mots connus.

- Attaque par tables pré-calculées (par exemple les rainbow tables). Cette attaque consiste à
calculer à l’avance 3 les empreintes cryptographiques d’un très vaste ensemble de mots de passe afin d’accélérer leur recherche, puis de comparer automatiquement chacune d’entre elles à une empreinte volée jusqu’à trouver une égalité qui prouvera que le mot de passe recherché a été trouvé.

- Attaque par ingénierie sociale. Cette attaque consiste à récupérer un mot de passe par des moyens détournés comme l’hameçonnage ou bien l’usurpation d’identité.

### Facteurs de possession:

Les principales menaces pesant sur les facteurs de possession sont le vol, la perte, la duplication, la falsification ou bien encore la compromission totale de l’équipement qui porte le facteur de possession. Afin de réaliser une usurpation d’identité, les attaquants vont chercher à récupérer les secrets cryptographiques contenus dans le facteur de possession via par exemple des attaques par canaux auxiliaires.

### Facteurs inhérent:

Les principales menaces pesant sur les facteurs inhérents (couramment appelés facteurs biométriques) visent à leurrer le mécanisme de reconnaissance biométrique en usurpant l’identité de la
personne physique, par exemple par la présentation d’une photographie ou d’une séquence vidéo préenregistrée ou altérée, ou d’un moulage de l’empreinte digitale.

**Authentification forte VS authentification multifacteur:**

Il convient de différencier authentification multifacteur et authentification forte.
D’une part, une authentification multifacteur est une authentification faisant intervenir plusieurs catégories
de facteurs.
Néanmoins, ces facteurs, pris indépendamment ou ensemble, ne sont pas forcément considérés comme étant forts (un exemple typique étant un mot de passe associé à un code temporaire reçu par SMS). D’autre part, une authentification forte (qui repose généralement sur un facteur unique) est une authentification reposant sur un mécanisme cryptographique dont les paramètres et la sécurité sont jugés robustes (l’élément secret est alors généralement une clé cryptographique).

Les protocoles d’authentification que l’on peut considérer comme forts reposent souvent sur des protocoles dits défi-réponse.
Le message envoyé par le prouveur pour s’authentifier dépend à la fois d’une clé secrète, mais aussi d’un défi variable envoyé par le vérifieur. Lorsqu’un prouveur souhaite prouver son identité à un vérifieur, ce dernier lui envoie alors un défi (une valeur aléatoire par exemple) et le prouveur doit lui transmettre une réponse calculée à partir de ce défi spécifique
(une signature de ce défi par exemple).

Afin d’être considérée comme forte, une authentification doit reposer sur un protocole cryptographique permettant de résister à certaines attaques comme :
- L’écoute clandestine (eavesdroppping en anglais), qui consiste pour un attaquant à passivement écouter le canal de communication entre le prouveur et le vérifieur.
-Les attaques par rejeu, qui consistent pour un attaquant à récupérer des informations d’authentification (comme un mot de passe ou son empreinte) et à utiliser ces informations pour les rejouer afin d’usurper l’identité de la cible (l’attaque pass-the-hash en est un exemple).
- Les attaques de l’homme-du-milieu, qui consistent pour un attaquant à intercepter et modifier
les communications se déroulant entre le prouveur et le vérifieur lors de l’authentification sans
être détecté.
-La non-forgeabilité : l’observation par un attaquant de plusieurs échanges d’authentification d’un
prouveur ne doit pas lui permettre d’usurper son identité dans un nouvel échange d’authentification.

Parmi les exemples d’authentification forte reposant sur un facteur de possession, on peut citer :
- L’authentification par certificats (stockés dans des cartes à puce par exemple).
- Les protocoles FIDO2 et FIDO U2F.
- Les protocoles d’OTP (One-Time Password) comme HOTP (HMAC-based OTP [32]), TOTP (Timebased OTP [34]) ou OCRA (OATH Challenge-Response Algorithm).

Dans chacun de ces cas, le prouveur prouve son identité au vérifieur en démontrant indirectement la possession d’une clé cryptographique qui doit rester secrète.

Parmi les exemples d’authentification forte reposant sur un facteur de connaissance, on peut citer :
- Le protocole Kerberos.
- Les protocoles de type PAKE (Password-Authenticated Key Agreement) comme SPAKE2 ou OPAQUE.

On peut ainsi différencier une authentification multifacteur « faible » d’une authentification multifacteur forte lorsque cette dernière fait intervenir au moins un facteur d’authentification considéré comme fort.

## Les classes d'attaques

### XSS :

Cross-Site Scripting, est une attaque visant la récupération des données de l’utilisateur (tel que son nom, prenom, information bancaire ect..). Elle à lieu par l’injection de donnée dans une page web, dans le but de provoquer un comportement particulier du navigateur qui va interpréter cette injection. De ce fait, ses injections ont la particularité d’être dans langages interpréter directement par la navigateur (ex : JavaScript ou HTML).
Ex :

*\<script>*
*window.location=’[http://www\_site\_dangereux\_et\_compromettant.com](http://www_site_dangereux_et_compromettant.com)’;*
*\</script>*

De ce fait je vous propose les recommandation sur lesquels nous comptons nous appuyer pour la réaliser du projet. Ces recommandations ont était étudié et traiter afin de choisir ici seulement celle qui vont avoir un effet de protection sur l’application contre les attaque XSS. Vous trouverez donc le détails des recommandations et de leur utilité contre les attaque XSS.
<br>
* R4 : Utiliser l’API DOM
La vulnérabilité XSS dépend de la méthode utilisée pour présenter les contenus aux utilisateurs.
*

Template String :
var ligne = \`
< th >$ { meteo . c i t y . name } < / th >
< td >$ { meteo . weather . tempera ture } < td >\` ;
/ / Risque XSS
var node = document . createElemen t ( ” t r ” ) ;
node . innerHTML = li g n e ;
/ / Risque XSS
document . getElementBy Id ( ’ di s pl a y−g ri d ’ ) . appendChild ( node ) ;

Dans ce cas de figure il est tout à fait possible que l’utilisateur entre comme valeur :

meteo . c i t y . name = ” < i f r ame s r c = \ ” h t tp : / / au t re . s i t e . web \ ” > ”

Ce contenu sera interprété dans ce contexte.

De ce fait, l’utilisation côté client de Template String ES6, présente une vulnérabilité par rapport à l’utilisation de la balise HTML < t e m p l a t e >.

<br>
Tans dis que dans le cas de l’utilisation de la balise HTML < t e m p l a t e >.

< t e m p l a t e id = 'ligne'>
< tr >
< th id='ville'>$température< /td>
< /tr>
< /template>

var template = document.querySelector('#ligne);
var ligne = template.cloneNode(true);
ligne.content.querySelector('#ville').textContent = meteo.city.name;
ligne.content.querySelecyor('#temperature').textContent = meteo.weather.temperature;
document.getElementById('display-grid').appendChild(ligne.content);

Ce contenu sera affiché par le navigateur seulement, il ne sera pas interprété.

L’utilisation côté client de Template String ES6, présente une vulnérabilité par rapport à l’utilisation de la balise HTML < template>.
<br>
* R5 : Dissocier clairement la composition des pages web

Il est recommandé de dissocier clairement les données (JSON), la structure (HTML), le style (CSS) et la logique (JavaScript) d’une page web afin de réduire le risque d’occurrence de vulnérabilités XSS.
<br>
* R8 : Vérifier la conformité des données issues de sources externes

L’en-tête non-standard X-XSS-Protection n’est plus préconisé pour se prémunir des vulnérabilités XSS. Cet en-tête permettait la configuration d’une heuristique de filtrage XSS implémentée par les navigateurs. L’augmentation de la surface d’attaque entraînée par l’implémentation de ce filtre, l’introduction de nouvelles vulnérabilités et l’existence de contournements font que le support de ce mécanisme est en cours de retrait par certains navigateurs et a déjà été retiré par d’autres.
<br>
* R9 : Proscrire l'usage de la fonction eval()

La fonction eval est dédiée à la transformation de chaîne de caractères en code JavaScript. L’usage de cette fonction doit être proscrit.

Les fonctions JavaScript permettant la modification de contenu par insertion de fragment interprétable sont des fonctions susceptibles d’injecter du code malveillant. L’usage de ces fonctions dans un site ou une application web augmente à la fois la probabilité d’apparition et l’impact d’une vulnérabilité XSS.
<br>
* R10 : Proscrire l'usage de constructions basées sur l'évaluation de code

Il est fréquent que les ressources utilisées, CSS, fontes ou JavaScript, soient externes au site consulté et hébergées par des Content Delivery Networks (CDNs) afin d’améliorer la disponibilité du site et d’économiser de la bande passante. Cette pratique présente cependant des risques car elle étend la surface d’attaque jusqu’aux CDNs. En effet, par défaut une ressource corrompue ne sera pas détectée et se diffusera sur tous les sites qui en font usage. L’utilisation d’un mécanisme de vérification de l’intégrité des ressources issues d’un CDN, tel que Subresource Integrity (SRI, [12]), permet de s’assurer que les fichiers de ressources actifs correspondent bien à ceux qui ont été audités et validés en phase d’intégration logicielle. Une meilleure maîtrise du contenu présenté aux utilisateurs limite la vulnérabilité au XSS en cas, par exemple, de compromission d’un CDN.
<br>
* R12 : Contrôler l'intégrité des contenus tiers

Dans le cas d’un site en HTTPS, il est recommandé de mettre en œuvre systématiquement le contrôle de l’intégrité des ressources via SRI afin de réduire le risque de vulnérabilité XSS, en particulier pour les contenus issus d’un CDN.
<br>
* R13 : Restreindre les contenus aux ressources fiables

Il est recommandé de mettre en œuvre CSP afin de présenter aux navigateurs une liste des sites reconnus comme présentant des ressources fiables et ainsi contribuer au principe de moindre privilège en réduisant le risque potentiel de vulnérabilité XSS.
<br>
* R15 : Interdire des contenus inline

Notons que, par l’interdiction de l’inclusion de code JavaScript et CSS inline (i.e. directement dans le HTML), CSP contribue à la réduction de la surface d’attaque et donc de la probabilité d’apparition d’une vulnérabilité XSS. En outre, son fonctionnement par déclaration des domaines atteignables réduit également l’exploitabilité de telles vulnérabilités (i.e. le post-XSS), puisqu’un attaquant ne pourra pas demander au navigateur de récupérer du code malveillant ou de divulguer une information si cela requiert l’accès à un site qui ne figure pas dans la liste d’autorisations.

<br>
### Clickjacking :

Le détournement de clic, ou clickjacking, est un type d’attaque dans lequel une page web trompeuse incite un utilisateur légitime à cliquer sur du contenu en apparence légitime qui le mène en réalité à effectuer des actions, à son insu, sur d’autres sites. Ces attaques sont en général mises en œuvre au moyen d’une page piégée incluant des cadres (iframes) invisibles qui pointent vers des sites légitimes sur lesquels l’utilisateur piégé a ouvert une session. La protection contre ce type d’attaques consiste en la mise en place de mécanismes qui interdisent au navigateur l’inclusion du site à protéger dans un site tiers au travers d’une frame ou iframe. La directive frame-ancestors de CSP est une contre-mesure au détournement de clic car elle permet de spécifier une liste d’origines depuis lesquelles le navigateur a le droit exclusif de charger le site protégé dans un cadre.

* R16 : Définir la directive default-src
La directive frame-ancestors n’est pas supportée par l’implémentation en balise HTML de CSP. La protection contre le clickjacking avec CSP implique sa mise en œuvre au moyen de l’en-tête HTTP dédié.
*

### CSRF :

Cross-Site Request Forgery, est une attaque qui consiste à à faire réaliser à une utilisateur des actions privilégiées sur une application autre que celle sur laquelle il est connecté. Afin de pouvoir réaliser cette attaque, l faut que l’utilisateur soit authentifié sur le site sur lequel il possède des droits. Cette attaque passe par la mise en place d’un site piège qui, lorsque un utilisateur ce connecte dessus, lui fait réaliser à son issu des actions sur un autre site sur lequel il a des droits.
Pour le contrer on ajoute des jetons CSRF, qui possède une valeur unique généré aléatoirement coté serveur et envoyé au client.
<br>
* R19 : Etudier les risques liés à la collecte de rapports CSP

Certaines fonctionnalités de la spécification HTML [23] permettent de demander au navigateur d’émettre des requêtes silencieuses sans passer par l’exécution de code JavaScript ou CSS. Comme tout comportement qui conduit le navigateur d’une victime à initier une connexion de manière silencieuse, ces requêtes sont potentiellement indésirables et présentent des risques allant de la fuite d’informations jusqu’à l’exploitation de failles CSRF en passant par la réalisation d’attaques par déni de service distribué (DDoS).
<br>
* R31 : Limiter le transit des cookies aux flux sécurisés

Dès lors que des cookies sont nécessaires et que le site ou l’application n’est accessible qu’en HTTPS, le flag Secure doit être utilisé. Enfin, l’attribut SameSite permet de réduire drastiquement la vulnérabilité aux attaques CSRF, dans la mesure où il permet d’indiquer au navigateur dans quelles conditions il est acceptable d’émettre un cookie en fonction du contexte de navigation en cours.

### SQLi :

est une injection de code SQL (langage pour les données). Cette attaque consiste en la transmission de code malveillant parmi les données entrantes. Cette attaque à généralement lieu dans des champs de formulaire. Lorsque cette attaque à lieu, elle occasionne la perte de contrôle sur les données en base de données, ce qui peut mener à être récupéré, ou modifié et/ou supprimé.
<br>
* R25 : Proscrire l'usage de l'API Web SQL Database

Interdire l’usage de l’API Web SQL Database, désormais obsolète.

### SRI :

Subresource Integrity, permet d’exposer via l’attribut intergrity le résultat attendu d’un hash.
Le SRI se met en place lors du chargement d’une ressource. Son objectif est de protégé en vérifiant le résultat reçu par rapport au résultat attendu d’une ressource. Dans le cas du chargement d’une ressource tel que bootstrap, le résultat possède une empreinte propre à lui, le SRI permet de vérifier si cette empreinte est bien celle attendu, dans le cas ou elle l’est, la page s’affiche correctement dans le cas ou l’empreinte est différente, le SRI bloque le chargement de la ressource.

La compromission des ressources applicatives : consiste en un changement sur le site ou sur l’application afin de partager une idée politique ou de dénigrer le propriétaire ou revendiquer l’attaque afin de montrer notre savoir-faire.
Point d’eau : Vise un tendre un piège aux utilisateurs habituels qui vont activer une charge de malveillance sur le site. Attaques discrète qui ferait en sorte de ne pas être repérer.
Cette attaque a pour but d’infecter l’ordinateur des utilisateurs habituel.

Le vol de données : Souvent à but lucratif, perte de confidentialité et atteinte à la réputation.
Vol de donnée, comme compte bancaire, nom, prénom, adresse ect…
Elle est réalisée dans un but souvent lucratif et aboutit la plupart du temps à des usurpations d’identité ou à des paiements frauduleux.

Le déni de service : a pour objet de rendre indisponible le site attaqué pour ses utilisateurs légitimes que ce soit par l’arrêt ou par un ralentissement considérable du service.

### La compromission des ressources applicatives :

Consiste en un changement sur le site ou sur l’application afin de partager une idée politique ou de dénigrer le propriétaire ou revendiquer l’attaque afin de montrer notre savoir-faire.
Point d’eau : Vise un tendre un piège aux utilisateurs habituels qui vont activer une charge de malveillance sur le site. Attaques discrète qui ferait en sorte de ne pas être repérer.
Cette attaque a pour but d’infecter l’ordinateur des utilisateurs habituel.

### Le vol de données :

Souvent à but lucratif, perte de confidentialité et atteinte à la réputation.
Vol de donnée, comme compte bancaire, nom, prénom, adresse ect…
Elle est réalisée dans un but souvent lucratif et aboutit la plupart du temps à des usurpations d’identité ou à des paiements frauduleux.

### Le déni de service :

Il a pour objet de rendre indisponible le site attaqué pour ses utilisateurs légitimes que ce soit par l’arrêt ou par un ralentissement considérable du service.

### Cookies

Traduction de cookies
    <span class="colour" style="color:var(--vscode-markdown-wysText)">« Cookie » signifie « biscuit » en anglais. Le terme actuel dérive de l’expression « magic cookies », qui désigne un paquet de données.</span>

Exemple d'utilisation :

De la même manière qu'une emprunte laisse une trace sur le sol, les cookies laissent la trace d'un passage sur un site web.

Definition:
    Les cookies furent inventés au milieu des années 1990 par les Américains John Giannandrea et Lou Montulli. Les cookies se présentent sous la forme de fichiers textes, qui sont automatiquement enregistrés par le navigateur sur le disque dur lorsqu’un visiteur se rend sur un site web. Les cookies ont été développés pour améliorer l’expérience de l’utilisateur, pour permettre aux sites web de se souvenir du passage de telle personne. Les cookies ont ainsi joué un rôle important dans le développement d’internet tel qu’on le connait aujourd’hui. Les cookies ne sont pas des logiciels malveillants ni des virus. Chaque cookie a une date de péremption, variable en fonction des sites.

A quoi servent les cookies ?

C’est simple : les cookies donnent des informations sur les préférences de la personne qui visite le site. Ce dernier est ainsi en mesure de reconnaitre et conserver des informations, par exemple le choix de la langue, les identifiants de connexion, les pages consultées ou par exemple le contenu d’un panier. Les cookies sont aussi utiles pour obtenir des statistiques sur le site web en question :
temps de consultation des pages, taux de rebond, clics… Tout ceci permet d’améliorer le trafic sur le site.

<span class="colour" style="color:var(--vscode-markdown-wysText)">Il existe aussi un autre type de cookies : les cookies tiers. Ces derniers possèdent un rôle très important pour la publicité ciblée. En effet, ce sont eux, en gardant en mémoire les pages que vous consultez, qui permettent ensuite l’affichage de publicités liées sur d’autres sites. Rien d’étonnant donc si vous remarquez des publicités pour des canapés sur votre fil Facebook après avoir consulté un site d’ameublement.</span>


Comment fonctionnent les cookies ?

Les cookies fonctionnent dans le cadre du protocole de transfert hypertexte (HTTP), qui est un protocole de communication entre le client (l’internaute) et le serveur (le site web). Les cookies sont insérés sous forme de code dans chaque requête qu’envoie le serveur d’un site. Les cookies sont enregistrés par le navigateur dans un seul fichier.

### Bug bounty
<br>
Definition:
    Bug bounty est une récompense monétaire donnée aux pirates éthiques pour avoir réussi à découvrir et à signaler une vulnérabilité ou un bogue au développeur de l'application.


