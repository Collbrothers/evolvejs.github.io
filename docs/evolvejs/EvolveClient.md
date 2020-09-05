# EvolveClient extends [EventEmitter](https://nodejs.org/events)

<h4>The Built Client which is returned after by the EvolveBuilder</h4>

> **Constructor**
- **Makes a new Instance of the Class...**
```js
new EvolveClient(token: string, options: ClientOptions);
```

### Properties

#### .token
> **The Token of the Bot Client**
>
> **Type: [String](miscs/CommonTypes.md)**

#### .options
> **The Client Options for your customized client**
>
> **Type: [ClientOptions](docs/evolvejs/ClientOptions.md)**

#### .guilds
> **The Cached Guilds which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, Guild>](docs/objex/Objex.md)**

#### .channels
> **The Cached Channels which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, Channel>](docs/objex/Objex.md)**

#### .users
> **The Cached Users which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, User>](docs/objex/Objex.md)**

#### .emojis
> **The Cached Emoji which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, Emoji>](docs/objex/Objex.md)**

#### .roles
> **The Cached Role which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, Role>](docs/objex/Objex.md)**

#### .messages
> **The Cached Messages which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, Message>](docs/objex/Objex.md)**

#### .api
> **The API Class instance, using it you can request all Rest API Endpoints implemented in the library**
>
> **Type: [API](docs/evolvejs/API.md)**

#### .oauth2
> **The Oauth2 Class instance, using it you can request oauth2 token and exchange token! It will be only initialized if you used .setSecret() in the EvolveBuilder**
>
> **Type: [Oauth2](docs/evolvejs/Oauth2.md)**

#### .ws
> **The Gateway Class Instance, this is the class in which the client logs in! And all the websocket events!**
>
> **Type: [Gateway](docs/evolvejs/Gateway.md)**

#### .secret
> **The Client Secret which is to be used for Oauth2 if you want!**
>
> **Type: [string](miscs/CommonTypes.md)**

#### .structures
> **The Structures Class instance using which you can extend and modify any structure you want!**
>
> **Type: [Structures](docs/evolvejs/Structures.md)**

#### .user
> **The ClientUser Class which consists of the partial user property**
>
> **Type: [ClientUser](docs/evolvejs/ClientUser.md)**