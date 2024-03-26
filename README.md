local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()


local Section = Tab:AddSection({
	Name = "Main"
})

--[[
Name = <string> - Main.
]]

local Tab = Window:MakeTab({
	Name = "Made by Abby",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - Made by Abby.
Icon = <string> - https://icons8.de/icon/38247/freebsd.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddButton({
	Name = "AFK",
	Callback = function()
      		print("button pressed")
  	end    
})

--[[
Name = <string> - Press to AFK.
Callback = <function> - The function of the button.
]]
