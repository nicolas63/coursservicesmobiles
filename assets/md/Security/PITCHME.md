+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%
@snap[north text-white span-100]
1. Authentification et Authorisation : 
@snapend

Ne pas confondre ! 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%
@snap[north text-white span-100]
1. Authentification 
@snapend

Qui-est ce ? 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%
@snap[north text-white span-100]
1. Authentification 
@snapend

4 types facteurs d'authentification : <br/>

 - Facteur mémoriel : ce qu'on sait (mot de passe, nom de parents, etc )
 - Facteur matériel : ce qu'on a (une clé, un badge)
 - Facteur corporel : ce qu'on montre (voix, empreinte)
 - Facteur réactionnel : ce qu'on sait faire (geste, signature)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%
@snap[north text-white span-100]
1. Authorisation 
@snapend

@snap[west]
![alt Text](assets/img/Approved.jpg)
@snapend

@snap[east span-70]
Que peut-on faire ? <br/>
A t'on le droit de ... ? 
@snapend

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. Sécurité tour d'horizon  : 
@snapend

Les différentes façon de sécuriser une appplication aujourd'hui
+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. prérequis : 
@snapend

![alt Text](assets/img/HTTP-HTTPS.jpg)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. Mot de passe : 
@snapend

![alt Text](assets/img/flow-cookie-session-large.jpg)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. Mot de passe : 
@snapend

https://haveibeenpwned.com/ <br/>
https://en.wikipedia.org/wiki/List_of_the_most_common_passwords

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. Double facteurs : 
@snapend

![alt Text](assets/img/double_factors.jpg)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. Token : 
@snapend

![alt Text](assets/img/flow-cookie-session-large.jpg)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2.  Token format : JWT 
@snapends

Exemples (https://jwt.io/)


+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. OAuth2 : Authorisation
@snapends

![alt Text](assets/img/DiagSeqImplicite.png)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. OAuth2 : Authorisation
@snapends

Autres types de flux OAuth2 (https://blog.axawebcenter.fr/2016/03/oauth-comprendre-loauth-2-0-par-lexemple/)

+++?image=assets/img/bg/blue.jpg&position=left&size=35% 100%
@snap[west text-white span-65]
2. Open ID </br> Connect 
@snapend


@snap[east span-65]
![alt Text](assets/img/flow.png)
@snapend

+++?image=assets/img/bg/blue.jpg&position=left&size=35% 100%
@snap[west text-white span-65]
2. Open ID </br> Connect 
@snapend

Open id Conntect vs Oauth <br/>


+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. Sécurité en asp.net core : 
@snapends

Gestion des utilisateurs, des rôles, etc

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. Sécurité en asp.net core : 
@snapends

Demo 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
4. Fournisseurs d'identité : 
@snapends

@css[text-blue](I)dentity @css[text-blue](A)ccess @css[text-blue](M)anagement  

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
4. Fournisseurs d'identité : Avantages
@snapends

- Gestion centralisé des utilisateurs 
- Mise en place de role commun sur plusieurs application 
- Pas besoin de refaire la mécanique d'authentification et d'authorisation sur chaque API 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
4. Fournisseurs d'identité : Que choisir 
@snapends

- En .net : Identity server 
- Keycloak 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
4. Fournisseurs d'identité : 
@snapends

Demo 

@snap[north text-white span-100]
4. Fournisseurs d'identité : 
@snapends

Et les API Gateways dans tous ca ? <br/>
![alt Text](assets/img/ApiGatewayWithIdentity.png)