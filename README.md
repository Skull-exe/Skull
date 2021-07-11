-- Farewell Infortality.
-- Version: 2.82
-- Instances:
local ScreenGui = Instance.new("ScreenGui")
local Maingui = Instance.new("Frame")
local ScriptBox = Instance.new("TextBox")
local Execute = Instance.new("TextButton")
local Close = Instance.new("TextButton")
local Open = Instance.new("Frame")
local Open_2 = Instance.new("TextButton")
--Properties:
ScreenGui.Parent = game.CoreGui

Maingui.Name = "Maingui"
Maingui.Parent = ScreenGui
Maingui.BackgroundColor3 = Color3.new(1, 1, 1)
Maingui.Position = UDim2.new(0.396897823, 0, 0.134724855, 0)
Maingui.Size = UDim2.new(0, 306, 0, 385)
Maingui.Visible = false
Maingui.Active = true
Maingui.Draggable = true



ScriptBox.Name = "ScriptBox"
ScriptBox.Parent = Maingui
ScriptBox.BackgroundColor3 = Color3.new(1, 1, 1)
ScriptBox.Position = UDim2.new(0.124183014, 0, 0.0987012982, 0)
ScriptBox.Size = UDim2.new(0, 229, 0, 229)
ScriptBox.Font = Enum.Font.SourceSans
ScriptBox.Text = "Script Here !"
ScriptBox.TextColor3 = Color3.new(0.992157, 0.901961, 0.2)
ScriptBox.TextSize = 50



Execute.Name = "Execute"
Execute.Parent = Maingui
Execute.BackgroundColor3 = Color3.new(1, 1, 1)
Execute.Position = UDim2.new(0.123336196, 0, 0.815673113, 0)
Execute.Size = UDim2.new(0, 229, 0, 50)
Execute.Font = Enum.Font.SourceSans
Execute.Text = "Execute !"
Execute.TextColor3 = Color3.new(0.992157, 0.901961, 0.2)
Execute.TextScaled = true
Execute.TextSize = 50
Execute.TextWrapped = true
Execute.MouseButton1Click:connect(function()
	loadstring(ScriptBox.Text)()
end)

Close.Name = "Close"
Close.Parent = Maingui
Close.BackgroundColor3 = Color3.new(1, 1, 1)
Close.BorderSizePixel = 0
Close.Position = UDim2.new(0.875817001, 0, 0, 0)
Close.Size = UDim2.new(0, 38, 0, 38)
Close.Font = Enum.Font.Arcade
Close.Text = "<---"
Close.TextColor3 = Color3.new(0, 0, 0)
Close.TextScaled = true
Close.TextSize = 14
Close.TextStrokeColor3 = Color3.new(1, 0, 0)
Close.TextWrapped = true
Close.MouseButton1Click:connect(function()
	Maingui.Visible = false
	Open.Visible = true
end)

Open.Name = "Open"
Open.Parent = ScreenGui
Open.BackgroundColor3 = Color3.new(1, 1, 1)
Open.Position = UDim2.new(0, 0, 0.641366243, 0)
Open.Size = UDim2.new(0, 123, 0, 48)

Open_2.Name = "Open"
Open_2.Parent = Open
Open_2.BackgroundColor3 = Color3.new(1, 1, 1)
Open_2.Size = UDim2.new(0, 123, 0, 48)
Open_2.Font = Enum.Font.SourceSans
Open_2.Text = "Open !"
Open_2.TextColor3 = Color3.new(0.992157, 0.901961, 0.2)
Open_2.TextScaled = true
Open_2.TextSize = 14
Open_2.TextWrapped = true
Open_2.MouseButton1Click:connect (function()
	Maingui.Visible = true
	Open.Visible = false
end)

-- Scripts:
