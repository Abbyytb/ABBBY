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
Callback = <function> - function afkCommand(thePlayer, cmd) 
    if isPedInVehicle(thePlayer) then 
        outputChatBox("You must be on foot to use this command.", thePlayer, 255, 255, 255) 
    else 
        if isPedOnGround(thePlayer) then 
            if getElementDimension(thePlayer) < 10 then 
                outputChatBox("You will be AFK in 5 seconds", thePlayer, 255, 255, 255) 
                setTimer( 
                    function() 
                        setElementDimension(thePlayer, math.random(10, 1000)) 
                        setElementFrozen(thePlayer, true) 
                    end, 5000, 1 
                ) 
            elseif getElementDimension(thePlayer) >= 10 and getElementDimension(thePlayer) <= 1000 then 
                outputChatBox("You will be returned to the main dimension in 5 seconds", thePlayer, 255, 255, 255) 
                setTimer( 
                    function() 
                        setElementDimension(thePlayer, 0) 
                        setElementFrozen(thePlayer, false) 
                    end, 5000, 1 
                ) 
            end 
        else 
            outputChatBox("You must be on the ground to use this command.", thePlayer, 255, 255, 255) 
        end 
    end 
end 
addCommandHandler("afk", afkCommand) 
  




]]
