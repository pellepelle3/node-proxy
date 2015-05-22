Node Proxy
===

- Config

Config
---

Go to the config tab and set it with 
You must white list every service you want to access to the outside world think of it like a firewall all outside traffic comes through here

```json
"list": {
        "router": { // this states if you want any custom domains to point to a service you must replace "." periods with "*" astrix
          "health1*localhost": "health"
        },
        "publish": ["health"], // you must list all services you want to access by the world
        "page404": "<html><head><style>h1{margin: auto; position: absolute; top: 0; left: 0; right: 0; bottom: 0; height: 100px; font-family: 'arial'; font-weight: 100; color: #555; text-align: center; }body{background:#000;}</style></head><body><h1>404 Not Found</h1></body></html>" // this a custom 404 page for things that dont exist
      }
```





