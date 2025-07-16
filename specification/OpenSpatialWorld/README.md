# Spatial World Provisioning

![objects](../figures/objects.svg)

## Core Requirements and Feature   

| Requirements | Feature |
| --- | --- | 
| Start interactve experience on given device | URL, URL#join, URL#join=aspect.id |
| Start follows experience on given device | URL#follow, URL#follow=aspect.id
| Start non-interactive prview on given device | URL#preview, #preview=aspect.id |

## API Level

| API | Level 1 | Level 2 | Level 3 | Level 4 | Level 5 |
| --- | --- | --- | --- | --- | ---  |
| world access | read | read | read | read | read  |
| user access |  | read | read/write | read/write | read/write  |
| view access |  | read | read | read/write | read/write  |
| portal access |  | read | read | read/write | read/write  |
| Node access |  |  | read | read/write, Asset links | read/write, Asset links & data  |


## OpenAPI spec 

Source 

[API](API.yaml) 

Preview 

[Preview](https://redocly.github.io/redoc/?url=https://raw.githubusercontent.com/WebOfWorlds/WoWAPI/refs/heads/main/specification/OpenSpatialWorld/API.yaml)
