Library = {}

local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Name = "Libraryyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyy"
ScreenGui.Parent = not game:GetService("RunService"):IsStudio() and game:GetService("CoreGui") or game:GetService("Players").LocalPlayer.PlayerGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

local IconList = loadstring(game:HttpGet('https://raw.githubusercontent.com/Dummyrme/Library/refs/heads/main/Icon.lua'))()
function gl(i)
	local iconData = IconList.Icons[i]
	if iconData then
		local spriteSheet = IconList.Spritesheets[tostring(iconData.Image)]
		if spriteSheet then
			return {
				Image = spriteSheet,
				ImageRectSize = iconData.ImageRectSize,
				ImageRectPosition = iconData.ImageRectPosition,
			}
		end
	end
	if type(i) == 'string' and not i:find('rbxassetid://') then
		return {
			Image = "rbxassetid://".. i,
			ImageRectSize = Vector2.new(0, 0),
			ImageRectPosition = Vector2.new(0, 0),
		}
	elseif type(i) == 'number' then
		return {
			Image = "rbxassetid://".. i,
			ImageRectSize = Vector2.new(0, 0),
			ImageRectPosition = Vector2.new(0, 0),
		}
	else
		return i
	end
end



function Library:CrateWindow(p)
	local Logo = p.Logo or nil
	local Title = p.Title or "Null"
	local Desc = p.Desc or ""
	

	local Main = Instance.new("Frame")
	local Header = Instance.new("Frame")
	local Line = Instance.new("Frame")
	local RightContainer = Instance.new("Frame")
	local ImageButton = Instance.new("ImageButton")
	local LeftContainer = Instance.new("Frame")
	local LogoUi = Instance.new("Frame")
	local ImageLabel = Instance.new("ImageLabel")
	local UICorner = Instance.new("UICorner")
	local UICorner_2 = Instance.new("UICorner")
	local TitleHeader = Instance.new("TextLabel")
	local DecsTitle = Instance.new("TextLabel")
	local UICorner_3 = Instance.new("UICorner")
	local Container = Instance.new("Frame")
	local TabsContainer = Instance.new("Frame")
	local UICorner_4 = Instance.new("UICorner")
	local ScrollingFrame = Instance.new("ScrollingFrame")
	local UIListLayout = Instance.new("UIListLayout")
	local TabFrame = Instance.new("Frame")
	local TabTitle = Instance.new("TextLabel")
	local ImageLabel_2 = Instance.new("ImageLabel")
	local Button = Instance.new("TextButton")
	local InTabContainer = Instance.new("Frame")
	local UICorner_5 = Instance.new("UICorner")
	local ScrollingFrame_2 = Instance.new("ScrollingFrame")
	local UIListLayout_2 = Instance.new("UIListLayout")
	local ButtonFrame = Instance.new("Frame")
	local ButtonTitle = Instance.new("TextLabel")
	local ImageLabel_3 = Instance.new("ImageLabel")
	local TextButton = Instance.new("TextButton")
	local UICorner_6 = Instance.new("UICorner")
	local ToggleFrame = Instance.new("Frame")
	local ToggleTitle = Instance.new("TextLabel")
	local Frame = Instance.new("Frame")
	local BG = Instance.new("Frame")
	local UICorner_7 = Instance.new("UICorner")
	local Button_2 = Instance.new("Frame")
	local UICorner_8 = Instance.new("UICorner")
	local Button_3 = Instance.new("TextButton")

	--Properties:

	Main.Name = "Main"
	Main.Parent = ScreenGui
	Main.AnchorPoint = Vector2.new(0.5, 0.5)
	Main.BackgroundColor3 = Color3.fromRGB(18, 18, 18)
	Main.BackgroundTransparency = 0.150
	Main.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Main.BorderSizePixel = 0
	Main.Position = UDim2.new(0.499401271, 0, 0.5, 0)
	Main.Size = UDim2.new(0.588023901, 0, 0.680933833, 0)
	Main.ZIndex = 2

	Header.Name = "Header"
	Header.Parent = Main
	Header.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Header.BackgroundTransparency = 1.000
	Header.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Header.BorderSizePixel = 0
	Header.Position = UDim2.new(-3.1076965e-08, 0, 0, 0)
	Header.Size = UDim2.new(1.00000012, 0, 0.122857146, 0)

	Line.Name = "Line"
	Line.Parent = Header
	Line.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
	Line.BackgroundTransparency = 0.650
	Line.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Line.BorderSizePixel = 0
	Line.Position = UDim2.new(3.10769614e-08, 0, 1.00000012, 0)
	Line.Size = UDim2.new(0.99999994, 0, -0.0172413811, 0)

	RightContainer.Name = "RightContainer"
	RightContainer.Parent = Header
	RightContainer.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	RightContainer.BackgroundTransparency = 1.000
	RightContainer.BorderColor3 = Color3.fromRGB(0, 0, 0)
	RightContainer.BorderSizePixel = 0
	RightContainer.Position = UDim2.new(0.613034606, 0, 0, 0)
	RightContainer.Size = UDim2.new(0.386965364, 0, 0.982758701, 0)

	ImageButton.Parent = RightContainer
	ImageButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	ImageButton.BackgroundTransparency = 1.000
	ImageButton.BorderColor3 = Color3.fromRGB(0, 0, 0)
	ImageButton.BorderSizePixel = 0
	ImageButton.Position = UDim2.new(0.760030985, 0, 0.124741413, 0)
	ImageButton.Size = UDim2.new(0.171547979, 0, 0.763361812, 0)
	ImageButton.Image = "http://www.roblox.com/asset/?id=10152135063"

	LeftContainer.Name = "LeftContainer"
	LeftContainer.Parent = Header
	LeftContainer.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	LeftContainer.BackgroundTransparency = 1.000
	LeftContainer.BorderColor3 = Color3.fromRGB(0, 0, 0)
	LeftContainer.BorderSizePixel = 0
	LeftContainer.Position = UDim2.new(3.10769614e-08, 0, 0, 0)
	LeftContainer.Size = UDim2.new(0.386965364, 0, 0.982758701, 0)

	LogoUi.Name = "Logo"
	LogoUi.Parent = LeftContainer
	LogoUi.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	LogoUi.BackgroundTransparency = 1.000
	LogoUi.BorderColor3 = Color3.fromRGB(0, 0, 0)
	LogoUi.BorderSizePixel = 0
	LogoUi.Size = UDim2.new(0.284210533, 0, 0.999999881, 0)

	ImageLabel.Parent = LogoUi
	ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	ImageLabel.BackgroundTransparency = 1.000
	ImageLabel.BorderColor3 = Color3.fromRGB(0, 0, 0)
	ImageLabel.BorderSizePixel = 0
	ImageLabel.Size = UDim2.new(1, 0, 1, 0)
	ImageLabel.Image = Logo

	UICorner.CornerRadius = UDim.new(1, 0)
	UICorner.Parent = ImageLabel

	UICorner_2.CornerRadius = UDim.new(1, 0)
	UICorner_2.Parent = LogoUi

	TitleHeader.Name = "TitleHeader"
	TitleHeader.Parent = LeftContainer
	TitleHeader.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TitleHeader.BackgroundTransparency = 1.000
	TitleHeader.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TitleHeader.BorderSizePixel = 0
	TitleHeader.Position = UDim2.new(0.284210533, 0, 0, 0)
	TitleHeader.Size = UDim2.new(0.716000021, 0, 0.5, 0)
	TitleHeader.Font = Enum.Font.SourceSans
	TitleHeader.Text = Title
	TitleHeader.TextColor3 = Color3.fromRGB(255, 255, 255)
	TitleHeader.TextScaled = true
	TitleHeader.TextSize = 14.000
	TitleHeader.TextWrapped = true

	DecsTitle.Name = "DecsTitle"
	DecsTitle.Parent = LeftContainer
	DecsTitle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	DecsTitle.BackgroundTransparency = 1.000
	DecsTitle.BorderColor3 = Color3.fromRGB(0, 0, 0)
	DecsTitle.BorderSizePixel = 0
	DecsTitle.Position = UDim2.new(0.284210593, 0, 0.500000119, 0)
	DecsTitle.Size = UDim2.new(0.716000021, 0, 0.378620774, 0)
	DecsTitle.Font = Enum.Font.SourceSans
	DecsTitle.Text = Desc
	DecsTitle.TextColor3 = Color3.fromRGB(255, 255, 255)
	DecsTitle.TextSize = 14.000

	UICorner_3.CornerRadius = UDim.new(0.0500000007, 0)
	UICorner_3.Parent = Main

	Container.Name = "Container"
	Container.Parent = Main
	Container.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Container.BackgroundTransparency = 1.000
	Container.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Container.BorderSizePixel = 0
	Container.Position = UDim2.new(0, 0, 0.165714279, 0)
	Container.Size = UDim2.new(1, 0, 0.834285736, 0)

	TabsContainer.Name = "TabsContainer"
	TabsContainer.Parent = Container
	TabsContainer.BackgroundColor3 = Color3.fromRGB(18, 18, 18)
	TabsContainer.BackgroundTransparency = 0.300
	TabsContainer.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TabsContainer.BorderSizePixel = 0
	TabsContainer.Position = UDim2.new(0, 0, -0.0205479451, 0)
	TabsContainer.Size = UDim2.new(0.2668024, 0, 0.976027369, 0)

	UICorner_4.CornerRadius = UDim.new(0.100000001, 0)
	UICorner_4.Parent = TabsContainer

	ScrollingFrame.Parent = TabsContainer
	ScrollingFrame.Active = true
	ScrollingFrame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	ScrollingFrame.BackgroundTransparency = 1.000
	ScrollingFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
	ScrollingFrame.BorderSizePixel = 0
	ScrollingFrame.Size = UDim2.new(1, 0, 1, 0)

	UIListLayout.Parent = ScrollingFrame
	UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
	UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
	UIListLayout.Padding = UDim.new(0.00999999978, 0)

	TabFrame.Name = "TabFrame"
	TabFrame.Parent = ScrollingFrame
	TabFrame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TabFrame.BackgroundTransparency = 1.000
	TabFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TabFrame.BorderSizePixel = 0
	TabFrame.Size = UDim2.new(1, 0, 0.067482397, 0)

	TabTitle.Name = "TabTitle"
	TabTitle.Parent = TabFrame
	TabTitle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TabTitle.BackgroundTransparency = 1.000
	TabTitle.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TabTitle.BorderSizePixel = 0
	TabTitle.Position = UDim2.new(0.412213713, 0, 0, 0)
	TabTitle.Size = UDim2.new(0.587786317, 0, 1, 0)
	TabTitle.Font = Enum.Font.Highway
	TabTitle.Text = "Main"
	TabTitle.TextColor3 = Color3.fromRGB(255, 255, 255)
	TabTitle.TextSize = 14.000
	TabTitle.TextWrapped = true
	TabTitle.TextXAlignment = Enum.TextXAlignment.Left

	ImageLabel_2.Parent = TabFrame
	ImageLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	ImageLabel_2.BackgroundTransparency = 1.000
	ImageLabel_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
	ImageLabel_2.BorderSizePixel = 0
	ImageLabel_2.Position = UDim2.new(2.32958669e-07, 0, 0, 0)
	ImageLabel_2.Size = UDim2.new(0.33831805, 0, 1, 0)
	ImageLabel_2.Image = "rbxassetid://102331017367323"

	Button.Name = "Button"
	Button.Parent = TabFrame
	Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Button.BackgroundTransparency = 1.000
	Button.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Button.BorderSizePixel = 0
	Button.Size = UDim2.new(1, 0, 1, 0)
	Button.ZIndex = 2
	Button.Font = Enum.Font.SourceSans
	Button.Text = ""
	Button.TextColor3 = Color3.fromRGB(0, 0, 0)
	Button.TextSize = 14.000

	InTabContainer.Name = "InTabContainer"
	InTabContainer.Parent = Container
	InTabContainer.BackgroundColor3 = Color3.fromRGB(18, 18, 18)
	InTabContainer.BackgroundTransparency = 0.300
	InTabContainer.BorderColor3 = Color3.fromRGB(0, 0, 0)
	InTabContainer.BorderSizePixel = 0
	InTabContainer.Position = UDim2.new(0.293279022, 0, -0.0205479451, 0)
	InTabContainer.Size = UDim2.new(0.692464411, 0, 0.976027369, 0)

	UICorner_5.CornerRadius = UDim.new(0.0500000007, 0)
	UICorner_5.Parent = InTabContainer

	ScrollingFrame_2.Parent = InTabContainer
	ScrollingFrame_2.Active = true
	ScrollingFrame_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	ScrollingFrame_2.BackgroundTransparency = 1.000
	ScrollingFrame_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
	ScrollingFrame_2.BorderSizePixel = 0
	ScrollingFrame_2.Position = UDim2.new(0, 0, 0.028070176, 0)
	ScrollingFrame_2.Size = UDim2.new(1, 0, 0.971929848, 0)
	ScrollingFrame_2.CanvasPosition = Vector2.new(0, 4)

	UIListLayout_2.Parent = ScrollingFrame_2
	UIListLayout_2.HorizontalAlignment = Enum.HorizontalAlignment.Center
	UIListLayout_2.SortOrder = Enum.SortOrder.LayoutOrder
	UIListLayout_2.Padding = UDim.new(0.00999999978, 0)

	ButtonFrame.Name = "ButtonFrame"
	ButtonFrame.Parent = ScrollingFrame_2
	ButtonFrame.BackgroundColor3 = Color3.fromRGB(36, 36, 36)
	ButtonFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
	ButtonFrame.BorderSizePixel = 0
	ButtonFrame.Position = UDim2.new(0.0367647074, 0, 0.115582973, 0)
	ButtonFrame.Size = UDim2.new(0.899999976, 0, 0.0649999976, 0)

	ButtonTitle.Name = "ButtonTitle"
	ButtonTitle.Parent = ButtonFrame
	ButtonTitle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	ButtonTitle.BackgroundTransparency = 1.000
	ButtonTitle.BorderColor3 = Color3.fromRGB(0, 0, 0)
	ButtonTitle.BorderSizePixel = 0
	ButtonTitle.Position = UDim2.new(0.0500000007, 0, 0, 0)
	ButtonTitle.Size = UDim2.new(0.632352948, 0, 1, 0)
	ButtonTitle.Font = Enum.Font.SourceSans
	ButtonTitle.Text = "Teleport"
	ButtonTitle.TextColor3 = Color3.fromRGB(255, 255, 255)
	ButtonTitle.TextSize = 20.000
	ButtonTitle.TextWrapped = true
	ButtonTitle.TextXAlignment = Enum.TextXAlignment.Left

	ImageLabel_3.Parent = ButtonFrame
	ImageLabel_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	ImageLabel_3.BackgroundTransparency = 1.000
	ImageLabel_3.BorderColor3 = Color3.fromRGB(0, 0, 0)
	ImageLabel_3.BorderSizePixel = 0
	ImageLabel_3.Position = UDim2.new(0.782352924, 0, 0, 0)
	ImageLabel_3.Size = UDim2.new(0.135294124, 0, 1, 0)
	ImageLabel_3.Image = "rbxassetid://90238093188663"

	TextButton.Parent = ButtonFrame
	TextButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextButton.BackgroundTransparency = 1.000
	TextButton.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TextButton.BorderSizePixel = 0
	TextButton.Size = UDim2.new(1, 0, 1, 0)
	TextButton.ZIndex = 2
	TextButton.Font = Enum.Font.SourceSans
	TextButton.Text = ""
	TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
	TextButton.TextSize = 14.000

	UICorner_6.CornerRadius = UDim.new(0.200000003, 0)
	UICorner_6.Parent = ButtonFrame

	ToggleFrame.Name = "ToggleFrame"
	ToggleFrame.Parent = ScrollingFrame_2
	ToggleFrame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	ToggleFrame.BackgroundTransparency = 1.000
	ToggleFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
	ToggleFrame.BorderSizePixel = 0
	ToggleFrame.Position = UDim2.new(0.00808818452, 0, 0.064809002, 0)
	ToggleFrame.Size = UDim2.new(0.899999976, 0, 0.0649999976, 0)

	ToggleTitle.Name = "ToggleTitle"
	ToggleTitle.Parent = ToggleFrame
	ToggleTitle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	ToggleTitle.BackgroundTransparency = 1.000
	ToggleTitle.BorderColor3 = Color3.fromRGB(0, 0, 0)
	ToggleTitle.BorderSizePixel = 0
	ToggleTitle.Position = UDim2.new(0.0500000007, 0, 0, 0)
	ToggleTitle.Size = UDim2.new(0.632352948, 0, 1, 0)
	ToggleTitle.Font = Enum.Font.SourceSans
	ToggleTitle.Text = "Automatic Farm"
	ToggleTitle.TextColor3 = Color3.fromRGB(255, 255, 255)
	ToggleTitle.TextSize = 20.000
	ToggleTitle.TextWrapped = true
	ToggleTitle.TextXAlignment = Enum.TextXAlignment.Left

	Frame.Parent = ToggleFrame
	Frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Frame.BackgroundTransparency = 1.000
	Frame.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Frame.BorderSizePixel = 0
	Frame.Position = UDim2.new(0.68235296, 0, 0, 0)
	Frame.Size = UDim2.new(0.31764707, 0, 1, 0)

	BG.Name = "BG"
	BG.Parent = Frame
	BG.BackgroundColor3 = Color3.fromRGB(62, 62, 62)
	BG.BorderColor3 = Color3.fromRGB(0, 0, 0)
	BG.BorderSizePixel = 0
	BG.Position = UDim2.new(0.268518269, 0, 0.190352678, 0)
	BG.Size = UDim2.new(0.509259284, 0, 0.565313339, 0)

	UICorner_7.CornerRadius = UDim.new(1, 0)
	UICorner_7.Parent = BG

	Button_2.Name = "Button"
	Button_2.Parent = Frame
	Button_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Button_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Button_2.BorderSizePixel = 0
	Button_2.Position = UDim2.new(0.264403403, 0, 0.163362116, 0)
	Button_2.Size = UDim2.new(0.25, 0, 0.646817327, 0)

	UICorner_8.CornerRadius = UDim.new(1, 0)
	UICorner_8.Parent = Button_2

	Button_3.Name = "Button"
	Button_3.Parent = ToggleFrame
	Button_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Button_3.BackgroundTransparency = 1.000
	Button_3.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Button_3.BorderSizePixel = 0
	Button_3.Size = UDim2.new(1, 0, 1, 0)
	Button_3.ZIndex = 2
	Button_3.Font = Enum.Font.SourceSans
	Button_3.Text = ""
	Button_3.TextColor3 = Color3.fromRGB(0, 0, 0)
	Button_3.TextSize = 14.000

end
