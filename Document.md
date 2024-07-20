# LostHUB GUI Library
Instructions for LostHUB v1.0.0

## Loading Library
```lua
local LostHUB = loadstring(game:HttpGet(('https://raw.githubusercontent.com/LosterXProductions/LostHUB/main/LostHUB%20v1.0.lua')))()
```
## Creating the main UI
```lua
LostHUB.CreateUI("18544048114") -- Change the backgrounds image with an ImageId
```
## Creating a Catagory
```lua
LostHUB.CreateCatagory("Catagory Name")
```
## Creating a Label
```lua
LostHUB.CreateLabel("Your Text Here")
```
## Creating a Button
```lua
LostHUB.CreateButton("Your Button", function()
	-- Code Here
end)
```
## Creating a Toggle
```lua
LostHUB.CreateToggle("Your Toggle", function(Toggle)
	if Toggle then
		-- Value when considered Off
	else
		-- Value when considered On
	end
end)
```
## Creating a Slider
```lua
LostHUB.CreateSlider("Your Slider Name", 0, 100, 50, function(Value)
  -- Value is the Sliders Current Value
end)

--[[
  The 0 will be your minimum slider value, set this to any value you please.
  The 100 will be your maximum slider value, set this to any value you please.
  The 50 will be your default slider value, set this to any value between your maximum and your minimum.
]]
```
## Adding a label in the About Catagory
```lua
LostHUB.AddLabelToAbout("Your Label text here")
```
