local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "Script by Abby🔑", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})

--[[
Name = <string> - Script by Abby
HidePremium = <bool> - Whether or not the user details shows Premium status or not.
SaveConfig = <bool> - Toggles the config saving in the UI.
ConfigFolder = <string> - config
IntroEnabled = <bool> - Whether or not to show the intro animation.
IntroText = <string> - Script for ...
IntroIcon = <string> - https://icons8.de/icon/17840/freebsd
Icon = <string> - https://icons8.de/icon/17840/freebsd
CloseCallback = <function> - (function) when close <string> Abby
]]

local Tab = Window:MakeTab({
	Name = "Tab 1",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - Main
Icon = <string> - https://icons8.de/icon/17840/freebsd
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]


local Section = Tab:AddSection({
	Name = "Main Section"
})

--[[
Name = <string> - Main Section:
]]

local Tab = Window:MakeTab({
	Name = "Tab 1",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
