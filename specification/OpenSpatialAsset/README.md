# Spatial Asset Provisioning 

## Core Requirements and Feature   

Core requirements enabled with simple, proven and robust [HTTP 1.1](https://datatracker.ietf.org/doc/html/rfc2616) feature plus some modern extensions.   

| Requirements | Feature |
| --- | --- | 
| Data Security | E2E authorization for data provisioning and validation ( [HTTP 1.1 authentication](https://datatracker.ietf.org/doc/html/rfc2616) + Modern SSO implementation ) |
| Data Change | Essential indication of data change (  [HTTP 1.1, etag](https://datatracker.ietf.org/doc/html/rfc2616#section-14.19) ) |
| Multi-format | Single- und Multi-format requests with and without content negotiation  ( [HTTP 1.1: Content Negotiation](https://datatracker.ietf.org/doc/html/rfc2616#page-71) ) |

### Model type definition

We expect the data to comply with the [RFC2077](https://datatracker.ietf.org/doc/html/rfc2077) model definition 

- **Orthogonal space**
  - Orthogonal system
  - Spatial (3 or more) and temporal dimensions
- **Model structure**
  - Models are composed of Objects
  - Objects are instantiated/transformed elements
  - Elements are local or extern linked data with aggregatio sematic (e.g. referencing a VRML and IGES )
- **Structured Data** 
  - Multidimensional structures
  - Conversion should be structure preserving

### Model type registration 

There is a gowing number of [IANA Registration](https://www.iana.org/assignments/media-types/media-types.xhtml#model) for model types which enable the multi format support.

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

## Optional Feature 

The following API feature are option and only provided in some implementation 

### Additon asset aspects 

Additional information provided in a separate data package

- Generator
- Copyright
- etag
- Formats
- 3D volume
- GeoPose

### Data Fragment adresssing

Links inside the (model) domain and fragments of data. URI Fragment standards allow to address sub-data

- [W3C Media Frment URI](https://www.w3.org/TR/media-frags/): Spatially-, temporally- and structure-based addressing schema
  - example.com/media/movie.mpg#xywh=100,100,10,10&t=10,20
  - example.com/media/movie.mpg#id=cap

- **Open Opportunity**: Missing “Model Fragment URI”: Spatially-, temporally- and structure-based addressing
	- example.com/model/434/#xyzwhz=100,100,100,20,20,20&t=10,20
   - example.com/model/434/#include=node.tire


## OpenAPI spec 

### Source 

[API](API.yaml) 

### Preview 

[Preview](https://redocly.github.io/redoc/?url=https://raw.githubusercontent.com/WebOfWorlds/WoWAPI/refs/heads/main/specification/OpenSpatialAsset/API.yaml)
