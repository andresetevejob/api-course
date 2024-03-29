# NODE JS

I - Installation de Express

```
 Créer un dossier mon api, à l'intérieur de dossier, saisissez les commandes suivantes : 
 - npm init (pour initialiser un projet node js, choisissez les réponses par défaut)
-  npm install express (pour installer express)
```


II - Première application

1 - Fichier d'application express
```
 créer un fichier app.js et à l'interieur ajouter le code suivant :

 const express = require('express');
 const app = express();

 module.exports = app;
```

2 - Fichier de démarrage du serveur

```
 créer un fichier server.js toujours dans votre dossier d'application et rajouter le code ci après

 const http = require('http');
 const app = require('./app');
 app.set('port',process.env.PORT || 3000);
 const server = http.createServer(app);
 server.listen(process.env.PORT || 3000);

```

3 - Pour répondre à une requête get

```
 // répondre avec hello world quand on reçoit une requête GET
 app.get('/',(req, res) => {
  res.send('hello world');
 });
```
Routes
Une route est définie comme suit:
app.method(path, handler)
- method: permet de définir la méthode HTTP de la
requête.
- path: permet de définir le chemin de la ressource
demandée.
- handler: représente la fonction qui va gérer la requête
lors de sa réception.


4 - Méthodes de l’objet réponse

- res.send('hello world');
- res.status(404).end();
- res.status(404).send('product not found.');
- res.json(json_object);
- res.redirect(301, 'http://example.com');

5 - Paramètres d’une requête HTTP

- Query params
```
 Query params d’une requête HTTP:
 // http://localhost:3000/?prenom=john&nom=doe
 app.get('/', (req, res) => {
   res.send(req.query.prenom);
 });
```

 - Path params
```
 pathParam d’une requête HTTP:
    // http://localhost:3000/john/doe
    app.get('/:prenom/:nom', (req, res) => {
      var prenom = req.params.prenom
      res.send('Salut ' + prenom + ’ !’);
    });
```

- Récuperer un corps de requête

