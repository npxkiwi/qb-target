# IKKE MIG DER HER LAVET DET

### Hvordan du bruger den


### Client
```
Client Side
for k, v in pairs(Config.DoorLocation) do
    exports['qb-target']:AddCircleZone(v.name, v.location, 0.4, {
        name = v.name, -- Info
        debugPoly = false, -- Show Poly
    }, {
        options = {
            {
                num = 1, -- Num
                type = 'server', -- Server, Client
                event = 'nt_houserobbery:checkinv', -- Event
                icon = 'fas fa-lock',  -- Icon
                label = 'Dirk låsen op', -- Text
                drawDistance = 1, -- Draw Distance
                drawColor = {255, 255, 255, 255}, -- Draw Color
                successDrawColor = {30, 144, 255, 255} -- Success Draw Color
            }
        },
        distance = 1
    })
end
```
### Config
```
Config.DoorLocation = {
    ['1'] = {name = 'House#1', location = vector3(347.83, -1255.43, 32.7)},
   ['2'] = {name = 'House#2', location = vector3(347.83, -1255.43, 32.7)},
}

```
