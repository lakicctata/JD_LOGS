<h4 align="center">
LAKICC TATA IGRICE
</h5>




<h4 align="center">
This is a server log script for FiveM, which is used to log certain actions that are being made in the server.
</h5>

### Requirements
- A Discord Server
- FiveM FXServer

### V1.1.1
- Added hex color code support. (Old decimal color codes will still work.)
- Added option to hide player info on exports. (Very simple just change the `PLAYER_ID` to `0` and it wont show any info.)

### V1.1.0
- Reworked Export function. (Now with identifier support)

### V1.0.4
- Added Nearest Postal For [This Postal Map](https://forum.cfx.re/t/release-postal-code-map-minimap-new-improved-v1-2/147458)
- Added check if the identifier is available ( Prevents some errors :slight_smile: )
- Fixed some small bugs

### V1.0.3
- Added Discord Identifier
- Added Steam Profile URL
- Fixed Death Reason
	- Player commited suicide
	- Player was murdered
	- Player Died (Other reasons like getting run over or random explosions)

### V1.0.2
- Added more Customizations
	- Bot's Username
	- Bot's Avatar
	- Embed Community Name
	- Embed Community Logo
	- Color settings for default Events
- Added Player ID to default Events
- Added Option to enable/disable Player ID
- Added option to enable/disable Steam ID

### V1.0.1
- Added option to disable Shooting Logs

### V1.0.0
- All log channel
- Log to seperate channels
- Log from server or client side
- Easy changeble Avatar and Username

# Download & Installation
lakicc tata igrice xd


1. Download the files
2. Put the JD_logs folder in the server resource directory
3. Add this to your `server.cfg`
```
ensure JD_logs
```

# Adding more logs

- Add the following code to your existing resource where you execude the code
```
exports.JD_logs:discord('MESSAGE_YOU_WANT_TO_POST_IN_THE_EMBED', PLAYER_ID, PLAYER_2_ID, 'DECIMAL_COLOR_CODE', 'WEBHOOK_CHANNEL')
```
- Create a discord channel with webhook and add this to the webhooks.
```
local webhooks = {
	all = "<DISCORD_WEBHOOK>",
	chat = "<DISCORD_WEBHOOK>",
	joins = "<DISCORD_WEBHOOK>",
	leaving = "<DISCORD_WEBHOOK>",
	deaths = "<DISCORD_WEBHOOK>",
	shooting = "<DISCORD_WEBHOOK>",
	resources = "<DISCORD_WEBHOOK>",
	<WEBHOOK_CHANNEL> = "<DISCORD_WEBHOOK>", <------
}
```

###  Discord ko ne udje gej: https://discord.gg/YbbhFBDDu3 

### Images
![JD_logs_Image](http://jokedevil.com/img/JD_logs.png)
