import discord
from discord.ext import commands

bot = commands.Bot(command_prefix='/')

@bot.event
async def on_ready():
    print(f'{bot.user.name} is ready.')

@bot.event
async def on_message(message):
    if message.content.lower() == 'sunucuescordu':
        await message.channel.send('Muhammed Ali Öcel')

bot.run('MTI1NTk5NDQxNTYwMDYzMTg1OQ.GQ2WcI.Uc1RzQVkhW2OssXyl3hhKapP4BLPihiRUYN7UY')
