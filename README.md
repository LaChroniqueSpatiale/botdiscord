# botdiscord
$ npm install --save discord.js

const Discord = require("discord.js");
const client = new Discord.Client();

client.on('ready', () => {
  console.log(`Logged in as ${client.user.tag}!`);
});

client.on('message', msg => {
  if (msg.content === 'ping') {
    msg.reply('Pong!');
  }
});

client.login('NDQxMzAwNTQ3ODA3NjA4ODMy.DiZSEw.kU-XKsxObriIQskHl9LBl3QHqxg');

$ node bot.js
