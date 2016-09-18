# prayer-app-api
This is the server side code for the prayer app. 


## prerequisites
- node and npm
- mongodb


## setup
In the config folder, add file parameters.json with the following format:

```
{
  "server": {
    "host": "127.0.0.1",
    "port": 3000
  },
  "database": {
    "host": "127.0.0.1",
    "port": 27017,
    "db": "YourDataBaseName",
    "username": "YourDataBaseUserName",
    "password": "YourDatabasePassword"
  },
  "key": {
    "privateKey": "YourPrivateKey",
    "tokenExpiration": 3600000,
    "tokenExpirationDescription": "1 hour"
  },
  "mail": {
    "email": "senderMail@website.com",
    "userName": "YourMailAccount",
    "password": "YourMailPassword"
  }
}
```


## developing
1. Run `npm install` to install server dependencies.
2. Run `mongod` in a separate shell to keep an instance of the mongodb daemon running.
3. Run `node index`.
