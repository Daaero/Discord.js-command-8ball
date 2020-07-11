const Discord = require('discord.js')

    module.exports = {

    run: async (message, args) => {
        let replies = [
        "your answersyour answers",
        "your answers"

        ];
    
        let result = Math.floor((Math.random() * replies.length));
    
        const embed = new Discord.MessageEmbed()
        .setColor('RANDOM')
        .addField(message.author.username ,replies[result])
         message.channel.send(embed)

        },
    name: '8ball',

}
