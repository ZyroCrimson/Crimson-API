# Player Added

Fires when a player is added to the game.
> Not really needed but it's useful anyway

### Parameters
| Name | Type | Default | Description |
|------|-------|--------|-------------|
| player | Player | | The ```Player``` that joined |

### Example Code

```lua
local api = require(0000).begin()
local players = api:Get("Players")

players.PlayerJoined:Connect(function(player)
   print(player.Name .. " has joined!")
end
```
