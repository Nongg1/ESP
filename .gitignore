--by Novaz5792

if (not _G.LoadedX) then 
    _G.LoadedX = true 
    getgenv().Workspace = game:GetService("Workspace")
    getgenv().RunService = game:GetService("RunService")
    getgenv().Players = game:GetService("Players")
    getgenv().RenderStepped = RunService.RenderStepped 
    getgenv().Stepped = RunService.Stepped 
    getgenv().Player = Players.LocalPlayer 
    getgenv().Character = Player.Character or Player.CharacterAdded:Wait() 
    getgenv().HumanoidRootPart = Character:WaitForChild("HumanoidRootPart")
    getgenv().Humanoid = Character:WaitForChild("Humanoid") 
    getgenv().Camera = Workspace.CurrentCamera

    Workspace:GetPropertyChangedSignal("CurrentCamera"):Connect(function()
        getgenv().Camera = Workspace.CurrentCamera 
    end)

    Player.CharacterAdded:Connect(function(character)
        getgenv().Character = character 
        getgenv().HumanoidRootPart = Character:WaitForChild("HumanoidRootPart")
        getgenv().Humanoid = Character:WaitForChild("Humanoid")
    end)
end 
