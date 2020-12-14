## Crimson API

Crimson API is an API created by Zyro Crimson used for [Roblox](https://www.roblox.com) development.

### Introduction

Crimson API includes basic functions and events that can be used to make development easier.

### Example Code (In a Server Script)
```lua
-- get the module from the module's id
local api = require(0000)
```

```lua
-- start the module
local api = require(0000)
api = api.begin() -- call the "begin" function 
```

```lua
-- send something to the ouput
local api = require(0000)
api = api.begin()

api.print("Hello World!") -- print something in the output
```

```lua
-- Example way to load a player's animation
local api = require(0000).begin()
local players = game:GetService("Players")

player.PlayerAdded:Connect(function(plr)
   local char = plr.Character or plr.CharacterAdded:Wait()

   -- make the player's avatar play an animation
   local track = api:Get("Animator"):LoadAnimation(character, "rbxassetid://")
end)
```
