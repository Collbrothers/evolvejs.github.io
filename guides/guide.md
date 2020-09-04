# Basic Usage Guide

> This is a simple bot to create a ping pong bot i.e. a bot that replies with pong when you message ping in a channel

```js
const { EvolveBuilder, GatewayIntent, CacheOptions } = require("@evolvejs/evolvejs");

const client = new EvolveBuilder()
                     .setToken("your bot token here pls")
                     .enableCache(CacheOptions.ALL)
                     .enableIntents(GatewayIntent.GUILD, GatewayIntent.GUILD_MESSAGES)
                     .build();

client.on("clientReady", () => console.log(client.user.username));
client.on("newMessage", (msg) => {
    if(msg.content === "ping") {
        msg.channel.send("Pong!")
    }
});
```