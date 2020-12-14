## Get

Get is a method used to get services from the ```API``` table.
> Services can also be indexed by API.\<service>

### Parameters

| Returns | Parameters | Description |
|---------|------------|-------------|
| Service | Get (string Service) | Returns a service from the ```API``` table |

### Example Code

```lua
local api = require(0000).begin()
local animatorService = api:Get("Animator")
```
