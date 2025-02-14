# JSON Server for CRM React.JS

package.json:

```
 "start": "node ./server.js",
```

server.js:

```
const jsonServer = require('json-server');
const server = jsonServer.create();
const router = jsonServer.router('data.json');
const middlewares = jsonServer.defaults();
const port = 8000;

server.use(middlewares);
server.use(router);

server.listen(port);
```

Запуск локально:

```
npx json-server --watch data.json --port 8000
```

### GiHub

<https://github.com/IgorMan2005/json-server-crm.git>


