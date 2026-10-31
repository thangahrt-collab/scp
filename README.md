local Players = game:GetService("Players").LocalPlayer 
local Character = Players.Character or Players.CharacterAdded:Wait()
local Tool = Character:FindFirstChildWhichIsA("Tool")

if Tool:FindFirstChild("Setting") then 
    local script = require(Tool:FindFirstChild("Setting"))
    script.Auto = true
    script.FlamingBullet = true
    script.CameraRecoilingEnabled = false
    script.AmmoPerMag = math.huge 
    script.IgniteChance = math.huge
    script.BaseDamage = math.huge
    script.FireRate = 0
    script.ReloadTime = 0 
    script.SpreadX = 0 
    script.SpreadY = 0
    script.BurstRate = 0
end    
