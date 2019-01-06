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
3. API RESTful
@snapend


### Utilidation des verbes HTTP : 

@css[text-blue](GET) : Récupération d'un resource<br/>
@css[text-blue](POST) : Création d'un resource<br/>
@css[text-blue](PUT) : Mise à jour d'un resource<br/>
@css[text-blue](DELETE) : Supression d'un resource<br/>

+++?image=template/img/bg/blue.jpg&position=top&size=100% 15%

@snap[north text-white span-100]
3. API RESTful
@snapend

### Utilidation des verbes HTTP : 

@css[text-blue](1XX) : Récupération d'un resource<br/>
@css[text-blue](2XX) : Création d'un resource<br/>
- 200 : OK 
- 201 : CREATED 
- 202 : NO Content 
@css[text-blue](3XX) : Mise à jour d'un resource<br/>
- 301 : Moved Permanently
- 302 : Found
- 304 : Not Modified

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

+++?image=assets/img/bg/blue.jpg&position=left&size=30% 100%

@snap[west text-white]
@size[3em](4.)
@snapend

@snap[north-east template-note text-gray]
Comment documenter une API ?
@snapend

### Utilisation de swagger

@snap[east span-70]
![Alt Text](assets/img/swagger-ui.png)
@snapend

+++?image=assets/img/bg/blue.jpg&position=left&size=30% 100%

@snap[west text-white]
@size[3em](4.)
@snapend

@snap[north-east template-note text-gray]
Comment versionner une API ?
@snapend

### Utilisation de swagger

@snap[east span-70]
![Alt Text](assets/img/swagger-ui.png)
@snapend