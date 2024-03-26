
})
Tab:AddBind({
	Name = "K",
	Default = Enum.KeyCode.K,
	Hold = false,
	Callback = function()
		print("press")
	end    
--[[
Name = <string> - The name of the bind.
Default = <keycode> - The default value of the bind.
Hold = <bool> - Makes the bind work like: Holding the key > The bind returns true, Not holding the key > Bind returns false.
Callback = <function> - The function of the bind.
]]

local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "Made by Abby", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})

--[[
Name = <string> - Made by Abby.
HidePremium = <bool> - Whether or not the user details shows Premium status or not.
SaveConfig = <bool> - Toggles the config saving in the UI.
ConfigFolder = <string> - The name of the folder where the configs are saved.
IntroEnabled = <bool> - Started Script...
IntroText = <string> - Script by Abby Discord.gg/abbyhub
IntroIcon = <string> - https://icons8.de/icon/38247/freebsd
Icon = <string> - URL to the image you want displayed on the window.
CloseCallback = <function> - Close Tab?.
]]

local Tab = Window:MakeTab({
	Name = "Main",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - Main
Icon = <string> - https://icons8.de/icon/38247/freebsd
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

local Section = Tab:AddSection({
	Name = "Main Section"
})

--[[
Name = <string> - Main Section
]]

Tab:AddButton({
	Name = "AFK",
	Callback = function()
      		print("button pressed")
  	end    
})

--[[
Name = <string> - Anti AFK
Callback = <function> - Make the player afk

]]
Tab:AddDropdown({
	Name = "Dropdown",
	Default = "1",
	Options = {"1", "2"},
	Callback = function(Value)
		print(Value)
	end    
})

--[[
Name = <string> - Auto Farming:
Default = <string> - 1
Options = <table> - Auto Farm Coins, Auto Farm Pet
Callback = <function> - The function of the dropdown.
]]
