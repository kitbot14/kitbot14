
config.js
```javascript
const config = {
  Discord: {
    tag: "2.0kit",
    id: "1248774218720743475",
    token: "MTI0ODc3NDIxODcyMDc0MzQ3NQ.8cE6694CL6Bus8jxDJmnCL6Bus8jxDJmn"
  },

  DiscordServer: {
    NinjaMod: "https://discord.gg/ninjamod",
    NinjaModHosting: "https://discord.gg/fH7w9GBW2d"
  },

  Site: {
    RedDom-vitrine: "https://red-dom.fr",
    RedDom-selfbot: "https://red-dom.fr/commands",
    RedDom-profile: "https://reddom.fun",
    RedDom-paste: "https://paste.red-dom.fr",
    RedDom-link: "https://link.red-dom.fr"
  }
};

module.exports = config;

```
index.js
```javascript
const Discord = require('discord.js');
const client = new Discord.Client();

client.once('ready', () => {
  console.log(`Bot connecté en tant que ${config.Discord.tag}`);
});

client.login(${config.Discord.token});
```
