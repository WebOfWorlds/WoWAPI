# Hello, Web Of Worlds !

Building a open, adaptive and connected Metaverse on modern web standards and feature :rocket: . 

# Foundation  

The Core Introduction [Core Introduction](https://metaverse-standards.org/#slides) to the [Metaverse Standards Forum](https://metaverse-standards.org) contains on the first slide the following statement that did not change for last years:

> The metaverse combines the **connectivity of the Web** with the **immersiveness** of **spatial computing**

A [MSF 3D Web Interoperability WG](https://metaverse-standards.org/domain-groups/3d-web-interoperability/)

# API Proposals

![Object Relation](specification/figures/objects.svg)

## Open Spatial World API


| API | Level 1 | Level 2 | Level 3 | Level 4 | Level 5 |
| --- | --- | --- | --- | --- | ---  |
| webApp access | single app | multi app | multi app | multi app | multi app  |
| user access |  | read | read/write | read/write | read/write  |
| view access |  | read | read | read/write | read/write  |
| portal access |  | read | read | read/write | read/write  |
| Node access |  |  | read | read/write, Asset links | read/write, Asset links & data  |


## Open Spatial Asset API

IANA [Registert](https://www.iana.org/assignments/media-types/media-types.xhtml#model) Model Encoding

| Name | [IANA Registration](https://www.iana.org/assignments/media-types/media-types.xhtml#model) | In domain Links |
| --- | --- | --- |
| 3mf | [model/3mf](https://www.iana.org/assignments/media-types/model/3mf) | |
| e57 | [model/e57](https://www.iana.org/assignments/media-types/model/e57) | |
| gltf-binary | [model/gltf-binary](https://www.iana.org/assignments/media-types/model/gltf-binary) | |
| gltf+json | [model/gltf+json](https://www.iana.org/assignments/media-types/model/gltf+json) | |
| JT | [model/JT](https://www.iana.org/assignments/media-types/model/JT) | jt |
| iges | [model/iges](https://www.iana.org/assignments/media-types/model/iges) | |
| mtl | [model/mtl](https://www.iana.org/assignments/media-types/model/mtl) | |
| obj | [model/obj](https://www.iana.org/assignments/media-types/model/obj) | |
| prc | [model/prc](https://www.iana.org/assignments/media-types/model/prc) | |
| step | [model/step](https://www.iana.org/assignments/media-types/model/step) | Any model format |
| step+xml | [model/step+xml](https://www.iana.org/assignments/media-types/model/step+xml) | Any model format |
| step+zip | [model/step+zip](https://www.iana.org/assignments/media-types/model/step-xml+zip) | Any model format |
| step-xml+zip | [model/step-xml+zip](https://www.iana.org/assignments/media-types/model/step-xml+zip) | Any model format |
| stl | [model/stl](https://www.iana.org/assignments/media-types/model/stl) | |
| u3d | [model/u3d](https://www.iana.org/assignments/media-types/model/u3d) | |
| vnd.usda | [model/vnd.usda](https://www.iana.org/assignments/media-types/model/vnd.usda) | usd |
| vnd.usdz+zip | [model/vnd.usdz+zip](https://www.iana.org/assignments/media-types/model/vnd.usdz+zip) | usd |
| x3d-vrml | [model/x3d-vrml](https://www.iana.org/assignments/media-types/model/x3d-vrml) | Any model format |
| x3d+fastinfoset | [model/x3d+fastinfoset](https://www.iana.org/assignments/media-types/model/x3d+fastinfoset) | Any model format |
| x3d+xml | [model/x3d+xml](https://www.iana.org/assignments/media-types/model/x3d+xml) | Any model format |
| [las](https://en.wikipedia.org/wiki/LAS_file_format) | 😦 | |
| [glExtRef](https://github.com/KhronosGroup/glTF-External-Reference) | 😦 | gltf |
| [SPZ](https://github.com/nianticlabs/spz) | 😦 | |

# Implementations

## Open Spatial World API

| Name | Liscene | Level | Asset Reference | Structure Provisioning |  
| --- | --- | --- | --- | --- | 
| x3domWorld | Free | 5  | gltf-binary, gltf+json, x3d+xml | x3d+xml |
| [threedy.io](https://www.threedy.io) | Commercial | 5 | e57, gltf-binary, gltf+json, JT, step, step+xml, step+zip, step-xml+zip, step-xml+zip, vnd.usda, vnd.usdz+zip, x3d-vrml, x3d+fastinfoset, x3d+xml, las | step+xml, x3d-vrml, x3d-vrml 
| HTMLModeWrapper | Free | 3  | vnd.usdz+zip | |
| UnrealWrapper | Free | 2 | |
| UnityWrapper | Free | 2 | |

## Open Spatial Asset API

| Name | Liscene | Format | 
| --- | --- | --- |
| [RapidPipeline](https://rapidpipeline.com) | Commercial | gltf-binary, gltf+json, vnd.usda, vnd.usdz+zip, x3d+xml |
| [Sketchfab](https://sketchfab.com) | Commercial | gltf-binary, gltf+json, vnd.usda, vnd.usdz+zip |

# Live Demo Worlds

| Name | Endpoint | API Level |
| --- | --- | --- |
| hello world | [testWorld.WebOfWorlds.io](https://testWorld.OpenSpatialWorld.io) | 3 | 
| open portal | [openPortal.WebOfWorlds.io](https://testWorld.OpenSpatialWorld.io) | 5 | 
| threedy industrial Metaverse Use-Case | [threedy.space/msf/60394sdf6/api/osw/v1](http://threedy.space/msf/60394sdf6/api/osw/v1) | 5 | 

# Standardisation
