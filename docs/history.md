# `History` Command

`/history <me/global>`

The `history` command allows you to view the last three generations either you have generated, or the global community has generated.

## Parameters

### `option` : **required**

The `option` parameter can be only one of two strings: `me` or `global`.

- `me` - Returns the last three generations you've created, in ascending order.
- `global` - Returns the last three generations anyone using the bot has created, in ascending order.

Examples:

`/history me`

`/history global`

### Output

The result of this command will be three embeds with the date of each generation, and the specific parameters used to generate the mission idea. The embed is ephemeral, meaning it can only be seen by you and won't spam the chat.

![history](https://imgur.com/BZLSgql.jpg)