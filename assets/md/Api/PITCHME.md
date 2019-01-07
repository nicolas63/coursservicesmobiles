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

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : URI  
@snapend

@css[text-blue](U)niform @css[text-blue](R)esource @css[text-blue](I)dentifier<br/>

![alt text](https://i.stack.imgur.com/mcTKf.jpg)

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](RE)presentational @css[text-blue](S)tate @css[text-blue](T)ransfer

 1. Uniforme
 2. Stateless
 3. Cacheable
 4. Client / Serveur : "Separation of Concerns"
 5. Layered

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](Uniforme)

L’interface est uniforme à tous les niveaux. Tous les éléments (et connecteurs) communiquent en utilisant la même interface.

Chaque ressource est identifiée de façon unique et canonicalisée avec son URL.

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](Stateless)

Une API REST ne doit pas maintenir de session.

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](Cacheable)

Il doit être possible de mettre les ressources en cache à tous les niveaux (front, connecteur intermédiaire, back, etc…)

Il doit être possible d’utiliser les implémentations standards de cache HTTP.

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](Client / Serveur : "Separation of Concerns")

L’API REST n’est pas concernée par l’affichage, les interactions utilisateur et la session

Tous ces éléments doivent être gérés par le client (Ex. : application web frontend)

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : REST 
@snapend

@css[text-blue](Layered)

La présence de “connecteurs” intermédiaires doit être implicite pour le client et le serveur (composant de cache / sécurité etc…)


+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Utilisation des verbes HTTP 
@snapend

@css[text-blue](GET) : Récupération d'une resource<br/>
@css[text-blue](POST) : Création d'une resource<br/>
@css[text-blue](PUT) : Mise à jour d'une resource<br/>
@css[text-blue](DELETE) : Supression d'une resource<br/>

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Utilisation des verbes HTTP 
@snapend

@css[text-blue](1XX) : Information<br/>
@css[text-blue](2XX) : Succès<br/>
- 200 : OK 
- 201 : CREATED 
- 202 : NO Content 
<br/>

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Utilisation des verbes HTTP  
@snapend

@css[text-blue](3XX) : Redirection<br/>
- 301 : Moved Permanently
- 302 : Found
- 304 : Not Modified

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

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

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Utilisation des verbes HTTP  
@snapend

@css[text-blue](5XX) : Erreur du client <br/>
- 500 : Internal Server Error
- 501 : Not Implemented
- 502 : Bad Gateway

[Et bien plus ...](https://fr.wikipedia.org/wiki/Liste_des_codes_HTTP)

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Niveau de maturité REST
@snapend

Richardson Maturity Model <br/>
![alt text](https://zestedesavoir.com/media/galleries/713/c34c43b3-955d-467f-ad3e-9f23ca42eec4.png)

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Niveau de maturité REST
@snapend

@css[text-blue](Niveau 0, le RPC sur HTTP en POX) (SOAP, XML-RPC) <br/>
![alt text](assets/img/level0.png)

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Niveau de maturité REST
@snapend

@css[text-blue](Niveau 0, L’utilisation de ressources différenciées)<br/>
![alt text](assets/img/level1.png)

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Niveau de maturité REST
@snapend

@css[text-blue](Niveau 2, L’utilisation des verbes et des codes retours HTTP)<br/>
![alt text](assets/img/level2.png)

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : Niveau de maturité REST
@snapend

@css[text-blue](Niveau 3, L’utilisation des contrôles hypermédia) <br/>
![alt text](assets/img/level3.png)


+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful : HATEOAS
@snapend

@css[text-blue](H)ypertext @css[text-blue](A)s @css[text-blue](T)he @css[text-blue](E)ngine @css[text-blue](O)f @css[text-blue](A)pplication @css[text-blue](S)tate

![alt text](https://zestedesavoir.com/media/galleries/713/c34c43b3-955d-467f-ad3e-9f23ca42eec4.png)


+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
1. Comment créer une API en asp.net core
@snapend


``` 
dotnet new webapi -o [NomDeVotreProjet]
```

+++ 

@snap[north text-white span-100]
4. Comment créer une API en asp.net core
@snapend

### Les controller 

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

@[1](Donne route de ce controller par défaut http://votredomain:port/api/NomDuController)
@[12-24](Récupération d'un item par sont id avec la route : /api/todo/1)


+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
4. Comment documenter une API ?
@snapend

### Utilisation de swagger

![Alt Text](assets/img/swagger-ui.png)


+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
5. Comment versionner une API ?
@snapend

Un paramètre dans le header : <br/>
services.AddApiVersioning(o => o.ApiVersionReader = new HeaderApiVersionReader("api-version"));

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

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
5. Comment versionner une API ?
@snapend

Directement dans l'url : /api/v1/maressource : <br/>
services.AddApiVersioning(o => o.ApiVersionReader =  new UrlSegmentApiVersionReader(); );

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
