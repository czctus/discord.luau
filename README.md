# discord.luau
*Note, I will not be updating this often.*
---
discord.lua is a Module for Roblox that allows for sending Webhook DM's easily.

## Why use this?
Well its easy to use.
Simply all you have to do is require the module, create a "Link", then make a "WebhookBuilder" object and send it.

Heres an example
```lua
local discordlua = require(path.to.discordlua)
local Link = discordlua.WebhookLink("https://discord.com/api/webhooks/xx/xx-xx-xx-xx")

local WebHookBuild = discordlua.WebhookBuilder()
	:SetContent(`Hello discord from Discord.Lua!\nIt is currently {os.date()}`)
	:SetName("My Webhook")

Link.Send(WebHookBuild)
```

## What features come with this?
Most of the Webhook features on the [Discord Docs](https://discord.com/developers/docs/resources/webhook) are available.
You can Edit, Execute, and even delete messages. Plus, more features will be coming soon.

## Great, How do i install?
1. Download the most recent RBXM/RBXMX from the [Releases](https://github.com/czctus/discord.luau/releases)
2. Drag and Drop the downloaded file into Roblox Studio
3. Move it anywhere and make a new script
4. Put `local discordlua = require(path.to.discordlua)` at the top and replace path.to.discordlua with the actual path.

Yay, We are done. 

## What is the point of this?
You dont need to understand HTTP Requests, as it does the work for you.
Infact, you dont need to know much other than requiring a module and variables, also calling functions.
