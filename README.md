const Discord = require('discord.js');
const bot = new Discord.Client();

const token = 'NjE5MDUwMTAwNjk3NTk1OTE1.XXEhkw.fSi1dGP1BSR0o4DWIkVfvVK4oik'
bot.on('ready', () => {
    console.log('This Bot is Online');
})

bot.on('guildMemberAdd', member => {
    
    const channel = member.guild.channels.find(channel => channel.name === "🤗🔸welcome");
    if (!channel) return;

   channel.send(`**Hey${member}, welcome to Patrix's Army!:confetti_ball:
SEND CLIPS HERE: patbrawlstars@gmail.com :sparkles:
Enjoy Your Stay** :fire:`)


});

bot.login(token);
