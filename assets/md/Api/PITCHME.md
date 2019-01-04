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

+++

---?image=assets/img/bg/blue.jpg&position=left&size=30% 100%
@snap[west text-white]
@size[3em](2.)
@snapend


@snap[north-east template-note text-gray]
Qu'est-ce qu'une API 
@snapend


@snap[east span-70]

@css[text-blue](A)plication @css[text-blue](P)rogramming @css[text-blue](I)nterface

Facade permettant d'exposé des données

@snapend

+++

---?image=assets/img/bg/blue.jpg&position=left&size=30% 100%
@snap[west text-white]
@size[3em](3.)
@snapend


@snap[north-east template-note text-gray]
Comment créer une API en asp.net core 
@snapend


@snap[east span-70]
```javascript
// Include http module.
var http = require("http");

// Create the server. Function passed as parameter
// is called on every request made.
http.createServer(function (request, response) {
  // Attach listener on end event.  This event is
  // called when client sent, awaiting response.
  request.on("end", function () {
    // Write headers to the response.
    // HTTP 200 status, Content-Type text/plain.
    response.writeHead(200, {
      'Content-Type': 'text/plain'
    });
    // Send data and end response.
    response.end('Hello HTTP!');
  });

// Listen on the 8080 port.
}).listen(8080);
```

@[1,2](You can present code inlined within your slide markdown too.)
@[9-17](Your code is displayed using code-syntax highlighting just like your IDE.)
@[19-20](Again, all of this without ever leaving your slideshow.)
@snapend