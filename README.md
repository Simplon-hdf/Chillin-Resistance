# Chillin-Resistance

Pour cette application , nous avons été confronté à différentes problèmatiques concernant la sécurité. Nous avons mis en oeuvre un process détaillé pour chaque grande partie importante que nous allons décrire ci-dessous. 

## Les requêtes et la sécurisation de l'API

En ce qui concerne les requêtes http, nous allons mettre en place un système de sécurisation qui va permettre d'éviter certaines attaques cibles, compte tenu du fait que le client va en permanence faire des requêtes vers nos APIs (application programming interface que l'on va créer afin d'appeler à la demande du client - lors du visionnage d'une vidéo - les vidéos stockées)lors des visionnages des différents cours proposés : 

- Cela commence par la configuration des CORS (Cross-origin resource sharing
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

Aujourd'hui la norme pour les requêtes HTTP est l'ajout du HSTS qui fait la transmission d’un en-tête HTTP lors de l’accès au site en HTTPS pour assurer son intégrité.

Il est obligatoire de posséder le protocole HTTPS afin de garantir la sécurité des données et de l'utilisation de l'application à l'utilisateur. La mise en place de HTTPS a pour objectif :
■ de garantir, autant que possible, l’authenticité du site consulté ;
■ de garantir également l’intégrité et la confidentialité des données échangées en bloquant les
attaques de type Man-In-The-Middle (écoute, interception ou modification des échanges à la
volée par des tiers, à l’insu de l’utilisateur).

Nous utiliserons également le protocole TLS, un protocole important de communication sur les réseaux et internet. Il permet une communication chiffrée entre un client et un serveur. Les données applicatives sont encapsulées de manière à assurer la confidentialité et l’intégrité des échanges. Le serveur est nécessairement authentifié, et des fonctions additionnelles permettent l’authentification du client lorsqu’un tel besoin a été identifié.C’est un protocole en poignée de main (Handshake) car le client et le serveur **négocie la connexion TLS**.
TLS est utilisé pour la connexion des sites HTTPS. Mais depuis, on trouve des déclinaisons par exemple avec les protocoles POP ou SMTP pour les serveurs mails.


