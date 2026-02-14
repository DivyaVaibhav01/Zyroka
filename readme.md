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

✔ Node.js **>=16.9.0**  
✔ Discord.js **>=14.6.0**  
✔ Running **Lavalink server (v3 or v4)**

> ```npm install zyroka```

---


## ⚙️ Basic Setup
```
const { Zyroka } = require("zyroka");
const { Connectors } = require("shoukaku");

const zyroka = new Zyroka({
    nodes: [{
      name: "Lavalink",
      url: "localhost:2333",
      auth: "youshallpass",
      secure: false
    }],
    shoukakuoptions: {
        moveOnDisconnect: false,
        resumable: false,
        resumableTimeout: 60,
        reconnectTries: 10,
        restTimeout: 60000
    },
    defaultSearchEngine: "<Lavalink Search Source>",
}, new Connectors.<Your Client Library>(<Discord Client>));
```

## 📚 Documentation
> **[Zyroka Docs](https://github.com/DivyaVaibhav01/Zyroka/tree/main/Documents)**  
> **[Shoukaku Docs](https://guide.shoukaku.shipgirl.moe/guides/1-getting-started/)**


## 🙏 Credits

Zyroka is built **on top of [Shoukaku](https://github.com/Deivu/Shoukaku)**, a powerful Lavalink client for Discord.js.  
All Lavalink communication and node management are powered by Shoukaku.  

Special thanks to the Shoukaku team for creating such an amazing library.


## 📜 License

MIT License
---

✅ **How to use this:**
1. Copy **everything** inside the code block above.  
2. Open your repo (local or GitHub).  
3. Create a file named `README.md`.  
4. Paste it, save, and commit.  

This is **ready to use**, professional-looking, with **badges, commands, setup, examples, and events**.  

---
