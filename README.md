local function getCenter()
    local frame = Instance.new("Frame")
    frame.Parent = game.CoreGui
    frame.Name = LocalPlayer.Name
    frame.AnchorPoint = Vector2.new(0.5,0.5)
    frame.Position = UDim2.fromScale(0.5,0.5)
    frame.Size = UDim2.fromOffset(10,10)
    frame.Visible = false
 
    return {frame.AbsolutePosition.X,frame.AbsolutePosition.Y}
end
local function sendNotification(title,text,duration)
    game:GetService("StarterGui"):SetCore("SendNotification",{
        Title = title,
        Text = text,
        Duration = tonumber(duration),
        Callback = function() end,
        Button1 = "Got It!"
    })
end
local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local main = libary:CreateWindow({
    Title = "Script made by Abby_ytb"
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
