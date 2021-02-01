import discord
from discord.ext import commands

client = commands.bot(command_prefix = '.')

@client.event
async def on_ready():
    print("Jacob's God bot is online!")

@client.event
async def on_member_join(member):
    print(f'{member] has entered this realm.')

@client.event
async def on_member_remove(member):
    print(f'{member} has vanished from this realm.')

client.run('ODA0NDM3Mjg4MzEzODE1MDYx.YBMUmw.gSXy5qc_aBikEO8mwG3oYpmsZho')
