# EvolveBuilder

<h4>The Main Class of EvolveJS, this is the class that creates up the EvolveClient for you!</h4>

> **Constructor**
- **Makes a new Instance of the Class (token is optional)...**
```js
new EvolveBuilder(token?: string);
```

### Methods

#### .setToken(token)
> **The Token for the EvolveClient**

**Parameter(s):**

|     Name      |                       Type                        |              Optional               |    Default    |    Description     |
| :-----------: | :-----------------------------------------------: | :---------------------------------: | :-----------: | :----------------: |
|   `token`   | [string]() | <span class="mdi mdi-close"></span> |    `undefined`     | The token for EvolveClient |

#### .enableCache(CacheOptions)
> **Enables the Cache Options**

**Parameter(s):**

|     Name      |                       Type                        |              Optional               |    Default    |    Description     |
| :-----------: | :-----------------------------------------------: | :---------------------------------: | :-----------: | :----------------: |
|   `cacheOptions`   | [CacheOptions]() | <span class="mdi mdi-check"></span> |    `Guild, channels and Users`     | The CacheOptions for EvolveClient |

#### .disableCache(CacheOptions)
> **Disables the Cache Options**

**Parameter(s):**

|     Name      |                       Type                        |              Optional               |    Default    |    Description     |
| :-----------: | :-----------------------------------------------: | :---------------------------------: | :-----------: | :----------------: |
|   `cacheOptions`   | [CacheOptions]() | <span class="mdi mdi-check"></span> |    `Guild, channels and Users`     | The CacheOptions to be **disabled** for EvolveClient |

#### .enableIntents(GatewayIntents)
> **Enables the Gateway Intents you want!**

**Parameter(s):**

|     Name      |                       Type                        |              Optional               |    Default    |    Description     |
| :-----------: | :-----------------------------------------------: | :---------------------------------: | :-----------: | :----------------: |
|   `gatwayIntents`   | [GatewayIntent]() | <span class="mdi mdi-check"></span> |    `GUILD, GUILD_MESSAGES, DIRECT_MESSAGES`     | The Gateway Intents for EvolveClient |

#### .disableIntents(GatewayIntents)
> **Disables the Gateway Intents you want!**

**Parameter(s):**

|     Name      |                       Type                        |              Optional               |    Default    |    Description     |
| :-----------: | :-----------------------------------------------: | :---------------------------------: | :-----------: | :----------------: |
|   `gatwayIntents`   | [GatewayIntent]() | <span class="mdi mdi-check"></span> |    `GUILD, GUILD_MESSAGES, DIRECT_MESSAGES`     | The Gateway Intents to be **disabled** for EvolveClient |

#### .setSecret(clientSecret)
> **Sets the Client Secret if you want to use Oauth2**

**Parameter(s):**

|     Name      |                       Type                        |              Optional               |    Default    |    Description     |
| :-----------: | :-----------------------------------------------: | :---------------------------------: | :-----------: | :----------------: |
|   `clientSecret`   | [string]() | <span class="mdi mdi-close"></span> |    `undefined`     | The Client Secret for EvolveClient |

#### .setShards(totalShard)
> **Total Number of shards of the client!**

**Parameter(s):**

|     Name      |                       Type                        |              Optional               |    Default    |    Description     |
| :-----------: | :-----------------------------------------------: | :---------------------------------: | :-----------: | :----------------: |
|   `totalShards`   | [number]() | <span class="mdi mdi-close"></span> |    `1`     | The Shards for EvolveClient |

#### .setActivity(activity)
> **Sets the client's activity**

**Parameter(s):**

|     Name      |                       Type                        |              Optional               |    Default    |    Description     |
| :-----------: | :-----------------------------------------------: | :---------------------------------: | :-----------: | :----------------: |
|   `activity`   | [Object]() | <span class="mdi mdi-close"></span> |    `Playing EvolveJS`     | The User Activity for EvolveClient |

#### .build()
> **Returns a built [EvolveClient](docs/evolvejs/EvolveClient.md)**

**Parameter(s):**

|     Name      |                       Type                        |              Optional               |    Default    |    Description     |
| :-----------: | :-----------------------------------------------: | :---------------------------------: | :-----------: | :----------------: |
|   `none`   | [undefined]() | <span class="mdi mdi-close"></span> |    `undefined`     | Returns built EvolveClient |