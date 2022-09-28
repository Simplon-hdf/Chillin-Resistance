# Chillin-Resistance

Pour cette application , nous avons été confronté à différentes problèmatiques concernant la sécurité. Nous avons mis en oeuvre un process détaillé pour chaque grande partie importante que nous allons décrire ci-dessous.

# Stratégie de Sécurisation d'une application🔒

    Mesures visant à empêcher le vol ou le piratage des données.

************************************************************************************************************

# a \ Sauvegarde
     Nous avons utilisé la sauvegaSimon-Libert/Chillin-Resistancerde (backup en anglais) pour dupliquer et à mettre en sécurité les données contenues dans le base de donnée de la'application.

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


