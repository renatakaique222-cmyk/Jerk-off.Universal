# Jerk-off.Universal
--This script wasn't made by anyone; I didn't make it. It belonged to my friend, but he stopped playing Roblox, so the script is now ownerless!



-- Создаем GUI с возможностью перетаскивания
local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Name = "CustomGUI"
ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

-- Основной фрейм GUI
local MainFrame = Instance.new("Frame")
MainFrame.Name = "MainFrame"
MainFrame.Size = UDim2.new(0, 200, 0, 150)
MainFrame.Position = UDim2.new(0.5, -100, 0.5, -75)
MainFrame.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
MainFrame.BorderSizePixel = 0
MainFrame.Parent = ScreenGui
MainFrame.Active = true
MainFrame.Draggable = true

-- Скругленные углы для фрейма
local UICorner = Instance.new("UICorner")
UICorner.CornerRadius = UDim.new(0, 10)
UICorner.Parent = MainFrame

-- Заголовок
local TitleLabel = Instance.new("TextLabel")
TitleLabel.Size = UDim2.new(1, 0, 0, 30)
TitleLabel.Position = UDim2.new(0, 0, 0, 0)
TitleLabel.BackgroundTransparency = 1
TitleLabel.Text = "jerk off by ???"
TitleLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TitleLabel.Font = Enum.Font.SourceSansBold
TitleLabel.TextSize = 20
TitleLabel.Parent = MainFrame

-- Кнопка закрытия (крестик)
local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 30, 0, 30)
CloseButton.Position = UDim2.new(1, -30, 0, 0)
CloseButton.BackgroundColor3 = Color3.fromRGB(200, 50, 50)
CloseButton.Text = "X"
CloseButton.TextColor3 = Color3.fromRGB(255, 255, 255)
CloseButton.Font = Enum.Font.SourceSansBold
CloseButton.TextSize = 18
CloseButton.Parent = MainFrame

-- Скругленные углы для кнопки закрытия
local CloseUICorner = Instance.new("UICorner")
CloseUICorner.CornerRadius = UDim.new(0, 5)
CloseUICorner.Parent = CloseButton

-- Кнопка R6
local R6Button = Instance.new("TextButton")
R6Button.Size = UDim2.new(0, 80, 0, 40)
R6Button.Position = UDim2.new(0, 20, 0, 50)
R6Button.BackgroundColor3 = Color3.fromRGB(60, 120, 255)
R6Button.Text = "R6"
R6Button.TextColor3 = Color3.fromRGB(255, 255, 255)
R6Button.Font = Enum.Font.SourceSansBold
R6Button.TextSize = 18
R6Button.Parent = MainFrame

-- Скругленные углы для кнопки R6
local R6UICorner = Instance.new("UICorner")
R6UICorner.CornerRadius = UDim.new(0, 8)
R6UICorner.Parent = R6Button

-- Кнопка R15
local R15Button = Instance.new("TextButton")
R15Button.Size = UDim2.new(0, 80, 0, 40)
R15Button.Position = UDim2.new(0, 100, 0, 50)
R15Button.BackgroundColor3 = Color3.fromRGB(60, 120, 255)
R15Button.Text = "R15"
R15Button.TextColor3 = Color3.fromRGB(255, 255, 255)
R15Button.Font = Enum.Font.SourceSansBold
R15Button.TextSize = 18
R15Button.Parent = MainFrame

-- Скругленные углы для кнопки R15
local R15UICorner = Instance.new("UICorner")
R15UICorner.CornerRadius = UDim.new(0, 8)
R15UICorner.Parent = R15Button

-- Тень для визуального эффекта
local Shadow = Instance.new("ImageLabel")
Shadow.Size = UDim2.new(1, 20, 1, 20)
Shadow.Position = UDim2.new(0, -10, 0, -10)
Shadow.BackgroundTransparency = 1
Shadow.Image = "rbxassetid://1316045217"
Shadow.ImageTransparency = 0.7
Shadow.ImageColor3 = Color3.fromRGB(0, 0, 0)
Shadow.ScaleType = Enum.ScaleType.Slice
Shadow.SliceCenter = Rect.new(10, 10, 118, 118)
Shadow.Parent = MainFrame
Shadow.ZIndex = -1

-- Функции для кнопок
CloseButton.MouseButton1Click:Connect(function()
    ScreenGui:Destroy()
end)

R6Button.MouseButton1Click:Connect(function()
    loadstring(game:HttpGet("https://pastefy.app/wa3v2Vgm/raw"))()
end)

R15Button.MouseButton1Click:Connect(function()
    loadstring(game:HttpGet("https://pastefy.app/YZoglOyJ/raw"))()
end)

-- Анимация наведения для кнопок
local function addHoverEffect(button)
    button.MouseEnter:Connect(function()
        button.BackgroundColor3 = Color3.fromRGB(80, 140, 255)
    end)
    button.MouseLeave:Connect(function()
        button.BackgroundColor3 = Color3.fromRGB(60, 120, 255)
    end)
end

addHoverEffect(R6Button)
addHoverEffect(R15Button)

-- Анимация наведения для кнопки закрытия
CloseButton.MouseEnter:Connect(function()
    CloseButton.BackgroundColor3 = Color3.fromRGB(255, 80, 80)
end)
CloseButton.MouseLeave:Connect(function()
    CloseButton.BackgroundColor3 = Color3.fromRGB(200, 50, 50)
end)
