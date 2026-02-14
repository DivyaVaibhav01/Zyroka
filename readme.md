<p align="center">
  <h1 align="center">Zyroka</h1>
  <p align="center">
    A modern, powerful Lavalink client for Discord bots with full queue support, advanced filters, multi-node stability & easy integration.
  </p>
</p>

---

## 🚀 Features

✅ Robust **music queue system** (add, skip, loop, shuffle, remove)  
✅ **Multi-node support** with auto reconnect & failover  
✅ **Spotify, YouTube & SoundCloud** search/playback support  
✅ **Advanced filters & effects** (bass boost, nightcore, speed control, EQ)  
✅ **Auto resume & reconnect** on disconnect  
✅ Easy integration with **Discord.js v14+**  
⚡ Full **event system** for player & node events

---

## 📦 Requirements

✔️ Node.js **>=16.9.0**  
✔ Discord.js **>=14.6.0**  
✔ Running **Lavalink server (v3 or v4)** :contentReference[oaicite:1]{index=1}

---

## 🛠️ Installation

**Install from npm**
```bash
npm install zyroka


const { Client, GatewayIntentBits } = require("discord.js");
const { Zyroka } = require("zyroka");
const { Connectors } = require("shoukaku");

const client = new Client({
  intents: [
    GatewayIntentBits.Guilds,
    GatewayIntentBits.GuildMessages,
    GatewayIntentBits.GuildVoiceStates,
    GatewayIntentBits.MessageContent
  ],
});

client.zyroka = new Zyroka({
  nodes: [
    {
      name: "MainLavalink",
      url: "localhost:2333",
      auth: "youshallpass",
      secure: false
    }
  ],
  defaultSearchEngine: "spotify",
  spotify: [
    {
      clientID: process.env.SPOTIFY_ID,
      clientSecret: process.env.SPOTIFY_SECRET
    }
  ],
  filters: {
    bassBoost: true,
    nightcore: false,
    pitch: 1.0
  }
}, new Connectors.DiscordJS(client));

client.login(process.env.TO
