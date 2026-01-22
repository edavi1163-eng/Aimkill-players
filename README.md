-- Creat painel Aim Kill
local player = game.Players.LocalPlayer
local gui = player.PlayerGui

-- Creat ScreenGui
local screenGui = Instance.new("ScreenGui")
screenGui.Name = "AimKill"
screenGui.Parent = gui

-- Creat Frame
local frame = Instance.new("Frame")
frame.Size = UDim2.new(0.2, 0, 0.4, 0)
frame.Position = UDim2.new(0.4, 0, 0.4, 0)
frame.BackgroundColor3 = Color3.new(0, 0, 0)
frame.BackgroundTransparency = 0.5
frame.Parent = screenGui
frame.Draggable = true
frame.Active = true

-- Título
local title = Instance.new("TextLabel")
title.Text = "Aim Kill"
title.Size = UDim2.new(0.8, 0, 0.2, 0)
title.Position = UDim2.new(0, 0, 0, 0)
title.BackgroundColor3 = Color3.new(0, 0, 0)
title.TextColor3 = Color3.new(1, 1, 1)
title.Parent = frame

-- Botão Minimizar
local minimizeButton = Instance.new("TextButton")
minimizeButton.Text = "-"
minimizeButton.Size = UDim2.new(0.2, 0, 0.2, 0)
minimizeButton.Position = UDim2.new(0.8, 0, 0, 0)
minimizeButton.Parent = frame
minimizeButton.MouseButton1Click:Connect(function()
    if frame.Size == UDim2.new(0.2, 0, 0.4, 0
