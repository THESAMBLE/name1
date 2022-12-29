-- be R15 and wear layered clothing
game.StarterGui:SetCore("SendNotification", {
    Title = "SCRIPT KAT";
    Text = "Made by RBLXdominations"; -- what the text says (ofc)
    Duration = 60;
})

local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()

local Window = Library.CreateLib("KAT", "BloodTheme")

local Tab = Window:NewTab("Home")
local Section = Tab:NewSection("Infomations")
Section:NewLabel("Script made by RBLXdominations")
Section:NewLabel("Scripts its for everyone")
Section:NewLabel("Discord comming soon")

local Tab = Window:NewTab("Scripts")
local Section = Tab:NewSection("Character")
Section:NewSlider("WalkSpeed", "More speed", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

Section:NewSlider("JumpPower", "More jump", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)

local Section = Tab:NewSection("Scripts hub")
Section:NewButton("CMD-X", "With cmd-x you can prite invisiblefling and you gonna trolling players", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/CMD-X/CMD-X/master/Source', true))()
end)

Section:NewButton("Infite yield", "With infite yield you can trolling players", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
end)

Section:NewButton("Orca", "Orca its strongth script", function()
    loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/richie0866/orca/master/public/latest.lua"))()
end)
