# SimpleDiscord
**SimpleDiscord** is a module that empowers developers to send messages, including text and embeds, directly to Discord channels, enhancing collaboration and productivity within Roblox Studio projects.

## Features
[details="Simple Installation"]
[spoiler]Do you think it's hard? Lol.[/spoiler]
[/details]

[details="In-Built Proxies"]
```lua
local WebhookUrl: string = "https://discord.com/api/webhooks/XXXXX/XXXXX"
local WebhookProxy: string = SimpleDiscord.Proxies.Lewi
local Webhook = SimpleDiscord.Webhook:Register(WebhookUrl, WebhookProxy)

Webhook:Send("Test Message with Proxy")
```
[/details]

[details="Easy Customisable Embeds"]
```lua
local Embed = SimpleDiscord.Embed:New()
		:SetTitle("You title here", "https://your-link.here")
		:SetDesc("Your description here.")
		:SetColour(SimpleDiscord.Colours.DefaultRed)
		:SetFields(
			SimpleDiscord.Embed:Field("Field Name 1", "Field Value 1"),
			SimpleDiscord.Embed:Field("Field Name 2", "Field Value 2"),
			SimpleDiscord.Embed:Field("Field Name 3", "Field Value 3")
		)
		:SetFooter("You footer text here", "https://your-image.here")
		:SetTimestamp(SimpleDiscord.Timestamp.now())
```
[/details]

## Documentation: [*soon*](https://github.com/KYRYLO-UA/SimpleDiscord/blob/main/README.md)

## Installation
* **Download** [any release of SimpleDiscord](https://github.com/KYRYLO-UA/SimpleDiscord/tree/main) or [SimpleDiscord Model (v1.0)|attachment](upload://1yeGrq1p1s1VITBzZpH4EDNwcwI.rbxm)

* **Place** this module script in **ReplicatedStorage**
![image|155x47](upload://tV3XxUY3WcSA8z1b60okEPrnFuo.png)

* **Create** new script in **ServerScriptService**
![image|201x47](upload://wqHERKtuk6zizcBTCUUCUwH4T0O.png)

* **Open** your created script
![image|339x62](upload://lo2TrdEuf8qwuVaELXNitI1VcEs.png)

* **Write** this code:
```lua
-- Services
local ReplicatedStorage = game:GetService("ReplicatedStorage")

-- Module
local SimpleDiscord = require(ReplicatedStorage.SimpleDiscord)
local SimplePresets = require(ReplicatedStorage.SimpleDiscord.Presets)

-- Webhook Registering
local WebhookUrl: string = "https://discord.com/api/webhooks/XXXXX/XXXXX"
local WebhookProxy: string = SimpleDiscord.Proxies.Lewi
local Webhook = SimpleDiscord.Webhook:Register(WebhookUrl, WebhookProxy)

-- Send Message from Presets
local Message = SimplePresets["TestPreset"]("lolkekarg")
Webhook:Send(Message)
```
* **Run** game.

* **Final!** You sent your first message to Discord from your Roblox game with **SimpleDiscord**.
![image|340x202](upload://fUKP3Ul4uj5HgG14dF3nCTgVsBv.png)


## Contributing
* **Discord**: @kyrylo.
* **Email**: [kirilljbicai@gmail.com](mailto:kirilljbicai@gmail.com)
