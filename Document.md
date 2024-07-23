# LostHUB GUI Library
Instructions for LostHUB Beta v1.1.1

## Loading Library
```lua
local LostHUB = loadstring(game:HttpGet(('https://raw.githubusercontent.com/LosterXProductions/LostHUB-GUI-Library/main/LostHUB%20Source')))()
```
## Creating the main UI
```lua
LostHUB.CreateUI({
	Name = "LosterX", -- The name of your UI
	Image = "18544048114", -- The ImageId for the background of your UI
	BackgroundColor = Color3.fromRGB(93, 0, 186) -- The background color of your UI
})
```
## Creating a Catagory
```lua
LostHUB.CreateCatagory({
	Name = "Catagory" -- Your catagories name.
})
```
## Creating a Label
```lua
LostHUB.CreateLabel({
	Text = "Text for Label."
})
```
## Creating a Button
```lua
LostHUB.CreateButton({
	Text = "Your Button",
	Function = function()
		print("Button Clicked")
	end,
})
```
## Creating a Toggle
```lua
LostHUB.CreateToggle({
	Text = "Your Toggle",
	Function = function(Toggle)
		if Toggle then
			game.Lighting.Ambient = Color3.fromRGB(106, 106, 106) -- Default Value
		else
			game.Lighting.Ambient = Color3.new(1, 1, 1) -- Value after Toggle enabled
		end
	end,
})
```
## Creating a Slider
```lua
LostHUB.CreateSlider({
	Text = "Your Slider",
	DefaultValue = 16,
	MinimumValue = 8,
	MaximumValue = 128,
	Function = function(Value)
		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value
	end,
})
```
## Notifying the User
```lua
LostHUB.NotifyLocalPlayer({
	Text = "They will see this at the top of their screen!"
})
```
## Adding a label in the About Catagory
```lua
LostHUB.AddLabelToAbout({
	Text = "Text for About me Section."
})
```
## Checking if the UI is already opened
```lua
LostHUB.CheckIfExecuted("UI-Name-Here", function()
	-- Your normal UI code here.
end)
```
