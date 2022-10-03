# `Generate` Command

`/generate <player team> [location] [objectives]`

The `generate` command is the primary feature of the Zeus Mission Generator bot. It allows you to produce a unique prompt by providing the bot with a few parameters.

**Note:** All parameters accept a maximum of **250 characters** each. There is a cooldown between generations (currently 4 seconds).

## Parameters

### `player_team` : **required**

The `player_team` option on the generate command is the only mandatory parameter. It specifies the protagonist team, or in other words the team your players will be playing as in the mission. You can provide both real and fictional units, but also providing description of the fictional unit may help the bot better understand the purpose of the unit.

Examples:

`/generate player_team:US Marines`

`/generate player_team:TMU, a Tactical Marine Unit branch of the Norweigian navy`

### `location` : **optional**

The first optional parameter is the `location` option which allows you to specify details about the setting your mission will take place in. Details can be related to the map itself, the geography, the time period, and even details such as weather. Locations can be absurd or unrelated to the unit specified, and the bot will try its best to make a coherent story out of it.

If you do not provide a location, a random map will be selected. The map can be one of the vanilla Arma 3 maps, the CUP maps, or some of the most popular workshop maps.

Examples:

`/generate player_team:US Marines location:An oil rig farm in the middle of the Kuwaiti desert, 1991`

`/generate player_team:NATO Forces location:A small village in the mountains of Altis at night`

`/generate player_team:Napoleon's army location:The moon`

### `objective` : **optional**

Another optional parameter is the `objective` option, which allows you to specify the goal of your `player_team` in the mission. Sometimes more detailed goals can result in more exciting ideas by the bot, but other times objectives that are too long can lead to the bot copy-pasting what you wrote as the mission idea.

If you do not provide an objective, a random one will be selected based on the list of objectives generated through the [Zeus Mission Gen](https://zeusmissiongen.com/) website.

`/generate player_team:US Marines objective:capture an HVT and take him to exfil point`

`/generate player_team:US Marines location:The Moon objective:find aliens`

### `task_list` : **optional**

The last optional parameter is the `task_list` option. Unlike the other parameters, this one only accepts a simple `True` or `False` value to specify whether you would like the bot to try and make a list of steps the player team must complete to achieve victory. The feature is in beta, but will soon become the standard generation method. 

Not including the parameter is the same as setting it to `False`. If you are only want a story idea and not the specific steps, feel free to not use this feature.

`/generate player_team:US Marines objective:destroy radio tower task_list:True`

## Output

Once the command is sent, the bot will take a moment to process the request and reply with an embedded idea generation. The embed will include all specified parameters (except `task_list`) and the generated prompt.

![generation1](https://imgur.com/gCpwZrd.jpg)
![generation2](https://imgur.com/7vkwUWj.jpg)
![generation3](https://imgur.com/G4FMwhK.jpg)
