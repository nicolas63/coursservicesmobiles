+++?image=assets/img/bg/blue.jpg&position=left&size=30% 100%
@snap[west text-white]
@size[3em](1.)
@snapend

@snap[north-east template-note text-gray]
Point sur le projet d'exemple 
@snapend

@snap[east span-70]
Mise en place de l'intégration continue sur gitlab <br/>
https://gitlab.iut-clermont.uca.fr/macheval/scoreuruniversel
@snapend

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
1. Point sur le projet d'exemple  : 
@snapend

Pour aller plus loin : <br/>
Déploiement continu <br/>
https://gitlab.iut-clermont.uca.fr/niraymon/siteclubinfo

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Enjeux
@snapend

- Protection des attaques
- Fiabilité 
- Monétisation
- Gestion des différents environnements (developpement, intégration, production)
- Gestion des différents clients (web, mobile, IOT, etc)

+++?image=assets/img/apilifecycle.png

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Importance
@snapend

Découpage en microservices :<br/>Multiplication des API 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Documentation et versionning
@snapend

Demo swagger 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Administration
@snapend

- Portail de management de l'api
- Enrôlement des services et nouvelles API 
- Pour les développeurs les informations dont ils ont besoins (statistiques)
- Gestion des droits 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Rate Limiting
@snapend

Limite du traffic pour ne pas surcharger l'infrastructure<br/>
Application de quotas

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Caching
@snapend

Permet des temps de réponse plus court<br/>

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Quality of service
@snapend

Rejoue les requêtes en échec 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Logging et Monitoring
@snapend

- Gestion des logs application et d'infrastructure
- Alertes (logs, healthcheck,etc)
- Monitoring

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%
@snap[north text-white span-100]
2. API Management : Logging et Monitoring
@snapend

Plusieurs stack technique : 
- ELK (@css[text-blue](E)lasticksearch @css[text-blue](L)ogstash @css[text-blue](K)ibana)
- TICK (@css[text-blue](T)elegraph @css[text-blue](I)nfluxDB @css[text-blue](C)ronograph @css[text-blue](K)apacitor)
- TIGK (@css[text-blue](T)elegraph @css[text-blue](I)nfluxDB @css[text-blue](G)rafana @css[text-blue](K)apacitor)

[Exemple de dashboard grafana](https://play.grafana.org)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Logging et Monitoring
@snapend

![alt Text](assets/img/TICK.png)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Load Balancer
@snapend

@snap[span-65]
![alt Text](assets/img/load-balancer.png)
@snapend

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Load Balancer
@snapend

Blue green deployment <br/>
Importance HealthCheck <br/>
[Exemple en asp.net core](https://docs.microsoft.com/fr-fr/dotnet/standard/microservices-architecture/implement-resilient-applications/monitor-app-health)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Load Balancer
@snapend

Demo docker 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
2. API Management : Service discovery
@snapend

Consultation et localisation des services disponibles <br/>
@css[text-blue](Consul)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%
@snap[north text-white span-100]
3. API Gateway 
@snapend

Qu'est-ce que c'est ? 

+++?image=assets/img/api-consumers.png

+++?image=assets/img/api-gw.png

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API Gateway : Ocelot 
@snapend

https://gitlab.iut-clermont.uca.fr/macheval/scoreuruniversel <br/>
https://ocelot.readthedocs.io/en/latest/introduction/gettingstarted.html

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API Gateway
@snapend

Kong, Gravitee,etc

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API Gateway : Pattern
@snapend

@css[text-blue](B)ackend @css[text-blue](F)or @css[text-blue](F)ront-End

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API Gateway : Pattern
@snapend

![alt Text](assets/img/BFF.png)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API Gateway + API management 
@snapend

En résumé c'est quoi ? 

+++?image=assets/img/apim.png


+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
Microservices : Asp.net core
@snapend

[eBook](https://aka.ms/microservicesebook) <br/>
[Exemple](https://github.com/dotnet-architecture/eshopOnContainers)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
Formation en ligne : 
@snapend

https://docs.microsoft.com/fr-fr/learn/

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
Conférence informatique :
@snapend

[Lavajug](https://www.lavajug.org/) <br/>
[MugInClermont](https://www.meetup.com/fr-FR/MugInClermont/) <br/>
[Clermont'ech](https://www.clermontech.org/)