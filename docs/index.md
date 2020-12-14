## Crimson API

Crimson API is an API created by Zyro Crimson used for [Roblox](https://www.roblox.com) development.

### Introduction

Crimson API includes basic functions and events that can be used to make development easier.

### Example Code (In a Server Script)
An example of what you can use the module for
```lua
-- Example way to load a player's animation
local api = require(0000).begin() -- require the module from the id and call the "begin" function to start it.
local players = game:GetService("Players")

players.PlayerAdded:Connect(function(plr)
   local char = plr.Character or plr.CharacterAdded:Wait()

   -- make the player's avatar play an animation
   local track = api:Get("Animator"):LoadAnimation(char, "rbxassetid://")
end)
```
