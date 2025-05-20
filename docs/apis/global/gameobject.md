# GameObject - Reference

#### Creating a GameObject
```lua
local exampleObject = CreateGameObject("Example!")
```

#### Setting the active state of a GameObject
```lua
SetActive(exampleObject, true) -- IF true the GameObject will be enabled, IF false the GameObject will be disabled.
```

#### Setting the parent of a GameObject
```lua
local worldPositionStays = true
SetParent(exampleObject, newParentObject, worldPositionStays)
```

#### Retrieving the name of a GameObject
```lua
local name = GetName(exampleObject)
```

#### Setting the position of a GameObject
```lua
--                 x  y  z
local newPosition = Vec3(0, 0, 0)
SetPosition(exampleObject, newPosition)
```

#### Finding a GameObject
```lua
local name = "GameObject name goes here"
local exampleObject = GetObject(name)
```

#### Creating a primitive GameObject
```lua
local primitive = "Cube" -- You can also do Capsule, Sphere, Plane and Quad.

-- Transform Variables
local position = Vec3(0, 0, 0)
local rotation = Quat(0, 0, 0, 0)
local scale = Vec3(1, 1, 1)

local exampleObject = CreatePrimitiveObject(name, position, rotation, scale)
```