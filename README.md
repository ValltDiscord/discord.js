
## Example usage

```js
const Discord = require('discord.js');
const client = new Discord.Bot();

client.on('ready', () => {
  console.log(`Logged in as ${client.user.tag}!`);
});

client.on('message', msg => {
  if (msg.content === 'ping') {
    msg.channel.send('pong');
  }
});

client.start('token');
```

