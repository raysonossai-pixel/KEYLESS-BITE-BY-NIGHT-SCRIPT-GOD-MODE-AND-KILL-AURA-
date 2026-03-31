# KEYLESS-BITE-BY-NIGHT-SCRIPT-GOD-MODE-AND-KILL-AURA-
Kill aura  God mode  Esp  Tp  Auto generators  Auto barricade  Speed  Inf stamina
code:local HttpService = game:GetService("HttpService")
local Players = game:GetService("Players")
local player = Players.LocalPlayer
local PlayerGui = player:WaitForChild("PlayerGui")

local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Parent = PlayerGui

local Frame = Instance.new("Frame")
Frame.Size = UDim2.new(0, 300, 0, 100)
Frame.Position = UDim2.new(0.5, -150, 0.5, -50)
Frame.BackgroundColor3 = Color3.fromRGB(54, 57, 63)
Frame.Parent = ScreenGui

local TextButton = Instance.new("TextButton")
TextButton.Size = UDim2.new(1, 0, 1, 0)
TextButton.BackgroundColor3 = Color3.fromRGB(114, 137, 218)
TextButton.TextColor3 = Color3.new(1, 1, 1)
TextButton.Font = Enum.Font.SourceSansBold
TextButton.TextSize = 24
TextButton.Text = "Join discord for script!"
TextButton.Parent = Frame

TextButton.MouseButton1Click:Connect(function()
    local url = "https://discord.gg/6jj4gMTGY"
    if syn and syn.request then
        syn.request({
            Url = url,
            Method = "GET"
        })
    end
    if setclipboard then
        setclipboard(url)
    end
    pcall(function()
        game:GetService("GuiService"):OpenBrowserWindow(url)
    end)
end)
