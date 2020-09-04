# EvolveClient extends [EventEmitter](https://nodejs.org/events)

<h4>The Built Client which is returned after by the EvolveBuilder</h4>

### Properties

#### .token
> **The Token of the Bot Client**
>
> **Type: [String]()**

#### .options
> **The Client Options for your customized client**
>
> **Type: [ClientOptions]()**

#### .guilds
> **The Cached Guilds which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, Guild>]()**

#### .channels
> **The Cached Channels which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, Channel>]()**

#### .users
> **The Cached Users which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, User>]()**

#### .emojis
> **The Cached Emoji which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, Emoji>]()**

#### .roles
> **The Cached Role which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, Role>]()**

#### .messages
> **The Cached Messages which were cached in the ClientReady Event (It will store if your CacheOptions is enabled in builder)**
>
> **Type: [Objex<string, Message>]()**

#### .api
> **The API Class instance, using it you can request all Rest API Endpoints implemented in the library**
>
> **Type: [API]()**

#### .oauth2
> **The Oauth2 Class instance, using it you can request oauth2 token and exchange token! It will be only initialized if you used .setSecret() in the EvolveBuilder**
>
> **Type: [Oauth2]()**

#### .ws
> **The Gateway Class Instance, this is the class in which the client logs in! And all the websocket events!**
>
> **Type: [Gateway]()**

#### .secret
> **The Client Secret which is to be used for Oauth2 if you want!**
>
> **Type: [string]()**

#### .structures
> **The Structures Class instance using which you can extend and modify any structure you want!**
>
> **Type: [Structures]()**

#### .user
> **The ClientUser Class which consists of the partial user property**
>
> **Type: [ClientUser]()**