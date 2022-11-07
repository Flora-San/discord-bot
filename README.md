simply configurations

[PyCharm](https://www.jetbrains.com/es-es/pycharm/)

[Python 3.9](https://www.python.org/downloads/)

also you can check if already have installed python in your computer with this command line

`python --version`


first create a new bot in [discord](https://discord.com/developers/docs/intro)

* Developer Portal --> Applications
* Click Button --> New Application
* add a name and create
* save the Token generated, probably we need later
* OAuth2 URL Generator -->   **.bot**
* Check all --> TEXT PERMISSIONS
* GENERATED URL--> open in a new window and select the server in add server
* click continue click authorize


run this command line in terminal to install discord 

` pip install discord
`

first configuration to run your own bot 

```
import discord
import random

from discord import Client

TOKEN = '-----PUT------YOUR-------TOKEN--------HERE--------'
#in this line you need to put the Token created previously for with your bot
client = discord.Client(intents=discord.Intents.default())


@client.event
async def on_ready():
    print('we have logged in as {0.user}'.format(client))


client.run(TOKEN)
```
