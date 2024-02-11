![image](https://github.com/KYRYLO-UA/SimpleDiscord/assets/60113306/282d8c82-a927-4d6c-89ab-31a212264ebf)# SimpleDiscord
**SimpleDiscord** is a module that empowers developers to send messages, including text and embeds, directly to Discord channels, enhancing collaboration and productivity within Roblox Studio projects.

## Features
* **Simple Installation**:
Do you think it's hard? Lol.

* **In-Built Proxies**:
```lua
local WebhookUrl: string = "https://discord.com/api/webhooks/XXXXX/XXXXX"
local WebhookProxy: string = SimpleDiscord.Proxies.Lewi
local Webhook = SimpleDiscord.Webhook:Register(WebhookUrl, WebhookProxy)

Webhook:Send("Test Message with Proxy")
```

* **Easy Customisable Embeds**:
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

## Documentation: [*soon*](https://github.com/KYRYLO-UA/SimpleDiscord/blob/main/README.md)

## Installation
* **Download** [any release of SimpleDiscord](https://github.com/KYRYLO-UA/SimpleDiscord/tree/main) or [SimpleDiscord Model (v1.0)|attachment](upload://1yeGrq1p1s1VITBzZpH4EDNwcwI.rbxm)

* **Place** this module script in **ReplicatedStorage**
* ![image](https://github.com/KYRYLO-UA/SimpleDiscord/assets/60113306/aa05360f-4a94-4a8c-898d-ce03b5d51dd7)

* **Create** new script in **ServerScriptService**
* ![image](https://github.com/KYRYLO-UA/SimpleDiscord/assets/60113306/f6affdbf-c6a6-4bde-9858-3d9709d7f2d8)

* **Open** your created script
* ![image](https://github.com/KYRYLO-UA/SimpleDiscord/assets/60113306/d59b000a-4f47-4ddd-a588-04afff8aa0af)

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
* ![image](https://github.com/KYRYLO-UA/SimpleDiscord/assets/60113306/fee81f7e-098b-436a-b4f0-10f7862fb7b5)

## Contributing
* **Discord**: @kyrylo.
* **Email**: [kirilljbicai@gmail.com](mailto:kirilljbicai@gmail.com)
