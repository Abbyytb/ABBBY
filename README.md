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

})
local farming = main:CreateTab({
    Name = "Farming",
    Icon = "rbxassetid://10709769841"
}) farming:CreateSection("Farming")
local egg = main:CreateTab({
    Name = "Egging",
    Icon = "rbxassetid://10723345518"
}) egg:CreateSection("Egging")
local teleports = main:CreateTab({
    Name = "Teleports"
}) teleports:CreateSection("Teleport")
local credits = main:CreateTab({
    Name = "Credits",
    Icon = "rbxassetid://10723396402"
}) credits:CreateSection("Credits")

