# `Export` Command

`/export [limit]`

The `export` command provides you with a downloadable JSON file that contains a limited history of your generations in ascending order, up to a maximum of 100 ideas.

**Note:** There is a 30 second cooldown between export requests.

## Parameters

### `limit` : **optional**

The `limit` parameter specifies how many ideas to include in the JSON file. You can enter an integer number no greater than the maximum limit of 100. 

Examples:

`/export`

`/export 25`

## Output

The output is a downloadable JSON file containing all your generations (up to the specified limit), their generation dates, and the parameters provided to create them. The result is ephemeral, meaning it can only be seen by you.

![exports](https://imgur.com/TekwGxv.jpg)