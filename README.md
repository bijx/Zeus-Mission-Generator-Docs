![alt text](https://imgur.com/RFULVHk.png)

# ZeusMissionGen 2.0

The Zeus Mission Generator 2.0 is a Discord Bot that uses the DaVinci GPT-3 AI model to generate unique mission story ideas, based on supplied parameters.

## Usage
[![alt](https://imgur.com/9u5PwQV.png)](https://discord.com/api/oauth2/authorize?client_id=1022558509558149131&permissions=2147576896&scope=applications.commands%20bot)

Once you've invited the bot to your server and given application command permissions (scoped in the invite link), you can use the following commands:

* `/generate <player team> [location] [objectives]` - Generate a mission story idea based on the supplied parameters:
  * `<player team>` - The unit the player is playing as. *(e.g. NATO, CSAT, AAF, custom, etc.)* **[REQUIRED]**
  * `[location]` - A description of the location of the mission. Can include time and details about the environment, and can be fictional. *(e.g. "A small village in the mountains of Altis", "A small town in the middle of Chernarus", "A small village in the mountains of Altis at night", etc.)* **[OPTIONAL]**
  * A description of the objective of the mission. *(e.g. "Defend the town from an attack by the CSAT", "Destroy the enemy base", "Rescue the hostages", etc.)* **[OPTIONAL]**
* `/info` - Get information about your user account such as:
  * `Tokens` - The number of generation tokens you have remaining. Each generation is worth 1 token.
  * `Total Generations` - The total number of generations you've produced.
* `/history <me/global>` - Shows either the last three prompts you've made or the last three prompts anyone globally has made.
* `/export [limit]` - Exports a JSON file containing a full history of prompts you've made (up to a maximum of 100). You can also specify a limit on how many of your last prompts you'd like to export.

## Report an Issue
If you'd like to request a new feature or report a bug, feel free to open a new issue ticket on the [issues]() page! 