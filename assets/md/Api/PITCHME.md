---?image=assets/img/bg/blue.jpg&position=left&size=30% 100%
@snap[west text-white]
@size[3em](1.)
@snapend

@snap[north-east template-note text-gray]
Présentation du projet et de la notation
@snapend

@snap[east span-70]
Un projet commun avec<br/>le cours de Windows phone<br/><br/>

[Une grille de notation](https://github.com/nicolas63/coursservicesmobiles/blob/Cours2019/Notation.md) <br/><br/>

[Un exemple de projet](https://gitlab.iut-clermont.uca.fr/macheval/scoreuruniversel)<br/>
@snapend


+++?image=assets/img/bg/blue.jpg&position=left&size=30% 100%
@snap[west text-white]
@size[3em](2.)
@snapend


@snap[north-east template-note text-gray]
Qu'est-ce qu'une API ?
@snapend


@snap[east span-70]

@css[text-blue](A)plication @css[text-blue](P)rogramming @css[text-blue](I)nterface

Note:

Facade permettant d'exposé des données => ici au travers de web services 

@snapend

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : URI  
@snapend

@css[text-blue](U)niform @css[text-blue](R)esource @css[text-blue](I)dentifier<br/>

![alt text](https://i.stack.imgur.com/mcTKf.jpg)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Le protocole HTTP  
@snapend

HTTP/0.9 (1990) : une ligne <br/>
```
GET /monfichier.html
```

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Le protocole HTTP  
@snapend

HTTP/1.0 (1991-1995) : Apparition des headers HTTP <br/>
```
200 OK
Date: Tue, 15 Nov 1994 08:12:31 GMT
Server: CERN/3.0 libwww/2.17
Content-Type: text/html
<HTML> 
Une page avec une image
  <IMG SRC="/monimage.gif">
</HTML>
```

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Le protocole HTTP  
@snapend

HTTP/1.1 (1997,1999,2014) : HTTP standardisé <br/>

Exemple de requête : <br/>
```
GET http://localhost/api/ressource HTTP/1.1
Accept : text/html
Content-Length: 11
User-Agent : Mozilla/4.0 (compatible; MSIE 5.0; Windows 95)

Contenu
```

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Le protocole HTTP  
@snapend

Exemple de réponse : <br/>
```
HTTP/1.1 200 OK
Content-Type : text/HTML
Content-Length : 1245

Contenu
```

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Le protocole HTTP  
@snapend

HTTP/2 (mai 2015) : Amélioration des performances <br/>
- Encodage binaire plutôt qu'en texte
- Multiplexé et donc plusieurs requêtes en parallèle
- Compression des en-têtes 
- En janvier 2018, 23.9% des sites web utilisent HTTP/2

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](RE)presentational @css[text-blue](S)tate @css[text-blue](T)ransfer

 1. Uniforme
 2. Stateless
 3. Cacheable
 4. Client / Serveur : "Separation of Concerns"
 5. Layered

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](Uniforme)

L’interface est uniforme à tous les niveaux. Tous les éléments (et connecteurs) communiquent en utilisant la même interface.

Chaque ressource est identifiée de façon unique et canonicalisée avec son URL.

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](Stateless)

Une API REST ne doit pas maintenir de session.

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](Cacheable)

Il doit être possible de mettre les ressources en cache à tous les niveaux (front, connecteur intermédiaire, back, etc…)

Il doit être possible d’utiliser les implémentations standards de cache HTTP.

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](Client / Serveur : "Separation of Concerns")

L’API REST n’est pas concernée par l’affichage, les interactions utilisateur et la session

Tous ces éléments doivent être gérés par le client (Ex. : application web frontend)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](Layered)

La présence de “connecteurs” intermédiaires doit être implicite pour le client et le serveur (composant de cache / sécurité etc…)


+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Utilisation des verbes HTTP 
@snapend

@css[text-blue](GET) : Récupération d'une ressource<br/>
@css[text-blue](POST) : Création d'une ressource<br/>
@css[text-blue](PUT) : Mise à jour d'une ressource<br/>
@css[text-blue](DELETE) : Supression d'une ressource<br/>

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Utilisation des verbes HTTP 
@snapend

@css[text-blue](1XX) : Information<br/>
@css[text-blue](2XX) : Succès<br/>
- 200 : OK 
- 201 : CREATED 
- 202 : NO Content 
<br/>

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Utilisation des verbes HTTP  
@snapend

@css[text-blue](3XX) : Redirection<br/>
- 301 : Moved Permanently
- 302 : Found
- 304 : Not Modified

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Utilisation des verbes HTTP  
@snapend

@css[text-blue](4XX) : Erreur du client <br/>
- 400 : Bad Request
- 401 : Unauthorized
- 403 : Forbidden
- 404 : Not Found
- 405 : Method Not Allowed
- 406 : Not Acceptable
- 415 : Unsupported Media Type

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Utilisation des verbes HTTP  
@snapend

@css[text-blue](5XX) : Erreur du serveur <br/>
- 500 : Internal Server Error
- 501 : Not Implemented
- 502 : Bad Gateway

[Et bien plus ...](https://fr.wikipedia.org/wiki/Liste_des_codes_HTTP)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Niveau de maturité REST
@snapend

Richardson Maturity Model <br/>
![alt text](https://zestedesavoir.com/media/galleries/713/c34c43b3-955d-467f-ad3e-9f23ca42eec4.png)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Niveau de maturité REST
@snapend

@css[text-blue](Niveau 0, le RPC sur HTTP en POX) (SOAP, XML-RPC) <br/>
![alt text](assets/img/level0.png)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Niveau de maturité REST
@snapend

@css[text-blue](Niveau 1, L’utilisation de ressources différenciées)<br/>
![alt text](assets/img/level1.png)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Niveau de maturité REST
@snapend

@css[text-blue](Niveau 2, L’utilisation des verbes et des codes retours HTTP)<br/>
![alt text](assets/img/level2.png)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Niveau de maturité REST
@snapend

@css[text-blue](Niveau 3, L’utilisation des contrôles hypermédia) <br/>
![alt text](assets/img/level3.png)


+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : HATEOAS
@snapend

@css[text-blue](H)ypertext @css[text-blue](A)s @css[text-blue](T)he @css[text-blue](E)ngine @css[text-blue](O)f <br/>
@css[text-blue](A)pplication @css[text-blue](S)tate

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : HATEOAS
@snapend

![alt text](assets/img/hateoassample.png)

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Type de contenu
@snapend

text/plain, application/xml, text/html, application/json, image/gif, image/jpeg , etc 

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Négociation de contenu
@snapend

2 HEADERS : <br/>

Content-Type: application/json <br/> permet de définir le contenu envoyé dans la requête <br/>
Accept: application/json <br/> permet de définir le contenu souhaité du client 


+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
4. Comment créer une API en asp.net core
@snapend


``` 
dotnet new webapi -o [NomDeVotreProjet]
```

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
4. Comment créer une API en asp.net core
@snapend

Les controller 

```csharp
[Route("api/[controller]")]
[ApiController]
public class TodoController : ControllerBase
{
    private readonly TodoContext _context;

    public TodoController(TodoContext context)
    {
        _context = context;
    }

    // GET: api/Todo/5
    [HttpGet("{id}")]
    public async Task<ActionResult<TodoItem>> GetTodoItem(long id)
    {
        var todoItem = await _context.TodoItems.FindAsync(id);

        if (todoItem == null)
        {
            return NotFound();
        }

        return todoItem;
    }
}
```

@[1](Donne la route de ce controller, par défaut http://votredomain:port/api/NomDuController)
@[12-24](Récupération d'un item par sont id avec la route : /api/todo/1)


+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
4. Comment documenter une API ?
@snapend

Utilisation de swagger

![alt Text](assets/img/swagger-ui.png)


+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
5. Comment versionner une API ?
@snapend

Un paramètre dans le header : <br/>
services.AddApiVersioning(o => o.ApiVersionReader = new HeaderApiVersionReader("api-version"));

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
5. Comment versionner une API ?
@snapend

```csharp
namespace Product.CommandService.Controllers.Product.V1
{
  [ApiVersion("1.0")]
  [Produces("application/json")]
  [Route("api/Product")]
  public class ProductController : Controller
  {
  }
}

namespace Product.CommandService.Controllers.Product.V2
{
  [ApiVersion("2.0")]
  [Produces("application/json")]
  [Route("api/Product")]
  public class ProductController : Controller
  {
  }
}
```

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
5. Comment versionner une API ?
@snapend

Directement dans l'url : @css[text-blue](/api/v1/maressource) : <br/>
services.AddApiVersioning(o => o.ApiVersionReader = new UrlSegmentApiVersionReader());

+++?image=assets/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
5. Comment versionner une API ?
@snapend

```csharp
[ApiVersion( "1.0" )]
[Route( "api/v{version:apiVersion}/[controller]" )]
public class HelloWorldController : Controller {
    public string Get() => "Hello world!";
}
 
[ApiVersion( "2.0" )]
[ApiVersion( "3.0" )]
[Route( "api/v{version:apiVersion}/helloworld" )]
public class HelloWorld2Controller : Controller {
    [HttpGet]
    public string Get() => "Hello world v2!";
 
    [HttpGet, MapToApiVersion( "3.0" )]
    public string GetV3() => "Hello world v3!";
}```
