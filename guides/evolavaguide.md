# EvoLava Guide
 
> A Simple Bot which will play music

```js
const { EvolveBuilder, GatewayIntents, CacheOptions } = require("@evolvejs/evolvejs");
const { EvoLavaClient } = require("@evolvejs/evolava")

const client = new EvolveBuilder()
                     .setToken("your bot token here pls")
                     .enableCache(CacheOptions.ALL)
                     .enableIntents(GatewayIntents.GUILD, GatewayIntents.GUILD_MESSAGES)
                     .build();

client.on("clientReady", () => {
    console.log(client.user.username);
    client.music = new EvoLavaClient(client, 
    [{
            host: "localhost",
            port: 2333,
            password: "youshallnotpass"
        }]
    );
});


client.on("newMessage", (msg) => {
    if(msg.content === "play") {
       const player = client.music.spawn({
            guild: msg.guild,
            voiceChannel: msg.member.voiceState.channel,
            textChannel: msg.channel,
            volume: 100,
            self: {
                mute: false,
                deaf: true
            }
        }, {
            repeatTrack: false,
            repeatQueue: false,
            skipOnError: true
        });

        const song = player.search("Rick Astley - Never Gonna Give you up", msg.member, options: {
            source: "yt",
            add: false
        });
 
        if(!song) return;
        player.queue.add(song);
        
        player.play();
    }
});
```