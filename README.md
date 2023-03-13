
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Robojini/Tuturial_UI_Library/main/UI_Template_1"))()

local Window = Library.CreateLib("Name", "RJTheme3")

local Tab = Window:NewTab("Main")

local Section = Tab:NewSection("Speed")

Section:NewSlider("Speed", "sliderInfo", 500, 0, function(s) -- 500 (Макс значение)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)



local Section = Tab:NewSection("Jump")

Section:NewSlider("Jump", "sliderInfo", 500, 0, function(s) -- 500 (Макс значение)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)

