
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Robojini/Tuturial_UI_Library/main/UI_Template_1"))()

local Window = Library.CreateLib("XickNak - Build a ship and find treasure", "RJTheme3")

local Tab = Window:NewTab("All")

local Section = Tab:NewSection("Speed")


Section:NewSlider("Speed", "SliderInfo", 500, 0, function(s) -- 500 (Макс. значение) | 0 (Мин. значение)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)


local Section = Tab:NewSection("Jump")


Section:NewSlider("JumpPower", "SliderInfo", 500, 0, function(s) -- 500 (Макс. значение) | 0 (Мин. значение)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)


local Section = Tab:NewSection("Gravity")


Section:NewSlider("Gravity", "SliderInfo", 196.2, 0, function(s) -- 500 (Макс. значение) | 0 (Мин. значение)
    game:GetService("Workspace").Gravity = s
end)


local Section = Tab:NewSection("Green")


Section:NewButton("Green", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").CamoTeam.Spawns.SpawnLocation.CFrame
end)


local Section = Tab:NewSection("White")


Section:NewButton("White", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").WhiteTeam.Spawns.SpawnLocation.CFrame
end)


local Section = Tab:NewSection("Blue")


Section:NewButton("Blue", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["Really blueTeam"].Spawns.SpawnLocation.CFrame
end)


local Section = Tab:NewSection("Black")


Section:NewButton("Black", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BlackTeam.Spawns.SpawnLocation.CFrame
end)


local Section = Tab:NewSection("Red")


Section:NewButton("Red", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["Really redTeam"].Spawns.SpawnLocation.CFrame
end)


local Section = Tab:NewSection("Magenta")


Section:NewButton("Magenta", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").MagentaTeam.Spawns.SpawnLocation.CFrame
end)


local Section = Tab:NewSection("Yellow")


Section:NewButton("Yellow", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["New YellerTeam"].Spawns.SpawnLocation.CFrame
end)


local Section = Tab:NewSection("Farm")


Section:NewButton("Farm", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.ForestStage.TerrainWall2.GrassPartTip.CFrame
	game:GetService("Workspace").Gravity = 0
	wait(1.5)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.CaveStage1.DarknessPart.CFrame
	wait(1.5)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.CaveStage2.DarknessPart.CFrame
	wait(1.5)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.CaveStage3.DarknessPart.CFrame
	wait(1.5)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.CaveStage4.DarknessPart.CFrame
	wait(1.5)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.CaveStage5.DarknessPart.CFrame
	wait(1.5)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.CaveStage6.DarknessPart.CFrame
	wait(1.5)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.CaveStage7.DarknessPart.CFrame
	wait(1.5)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.CaveStage8.DarknessPart.CFrame
	wait(1.5)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.CaveStage9.DarknessPart.CFrame
	wait(1.5)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.CaveStage10.DarknessPart.CFrame
	wait(1.3)
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").BoatStages.NormalStages.TheEnd.GoldenChest.LightPart.CFrame
	game:GetService("Workspace").Gravity = 194
	end)


	local Section = Tab:NewSection("Boat Motor Speed")


	Section:NewSlider("Speed", "SliderInfo", 500, 50, function(s) -- 500 (Макс. значение) | 0 (Мин. значение)
    game.Workspace.BoatMotor.MaxSpeed.Value = s
end)


local Section = Tab:NewSection("Boat Turning Speed")


	Section:NewSlider("Speed", "SliderInfo", 500, 1,function(s) -- 500 (Макс. значение) | 0 (Мин. значение)
    game.Workspace.BoatMotor.TurningSpeed.Value = s
end)


local Section = Tab:NewSection("Un Water Damage")


Section:NewButton("Un Water Damage", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.WaterDetector:Destroy()
end)


local Section = Tab:NewSection("Health")


    Section:NewSlider("Health", "SliderInfo", 500, 100,function(s)
    game.Players.LocalPlayer.Character.Humanoid.Health = s
	game.Players.LocalPlayer.Character.Humanoid.HealthDisplayDistance = s
	game.Players.LocalPlayer.Character.Humanoid.MaxHealth = s
end)


local Section = Tab:NewSection("Sit")


Section:NewButton("Sit", "ButtonInfo", function()
    game.Players.LocalPlayer.Character.Humanoid.Sit = true
end)
