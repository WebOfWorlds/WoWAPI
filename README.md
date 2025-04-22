# Hello, Web Of Worlds !

Building a open, adaptive and connected Metaverse on modern web standards and features :rocket: . 

# Foundation  

The [Metaverse Standards Forum](https://metaverse-standards.org) is today an essential and fundamental platform for the coordination of Metaverss standards, as it can incorporate coordinated requirements of SDOs, companies and end users. The [Core Introduction](https://metaverse-standards.org/#slides) contains the following statement on the first slide, which has not changed in recent years:

> The metaverse combines the **connectivity of the Web** with the **immersiveness** of **spatial computing**

There is a growing number of [Active Domain Groups](https://metaverse-standards.org/domain-groups/) and one with the focus on [3D Web Interoperability WG](https://metaverse-standards.org/domain-groups/3d-web-interoperability/)



A [Linked Spatial Experiences: The Web of Worlds](https://metaverse-standards.org/news/blog/linked-spatial-experiences-the-web-of-worlds/)

## Web of Wolrds Core Principles

This project to link virtual worlds highlights a compelling analogy between the World Wide Web—a unified system of URL-addressable, interconnected interactive experiences—and what we envision as a cohesive metaverse platform. This platform would consist of numerous addressable and linked spatial experiences, or virtual worlds, collectively forming what we call the “Web of Worlds.” Just as websites create a networked digital ecosystem, these spatial-first experiences would interconnect to create a seamless virtual universe as shown in Figure 1.

![Web Of Worlds](specification/figures/wow.svg)

We envision the “Web of Worlds” to be build on the current web infrastructure and support the following core requirements:

1. Unified Addressing System
* A single URI pointing to each discrete virtual world and functioning as a link between worlds
* Persistent data references in linked data environments
* Capability to store URIs/URLs for later access
* Simple URI sharing with additional users

2. Universal Experience Accessibility
* The "Web of Worlds" should be accessible through any standard browser
* Sharing of interactive spatial experiences rather than just isolated 3D data assets
* Web app-controlled user experiences as the dominant delivery model, i.e., use of client data vs. remote rendering

3. Rich Spatial Experiences
* Comprehensive user experiences for spatial data of any composition and size
* Support for both static and dynamic spatial data composition
* Capability to handle billions of addressable spatial data states
* High visual efficiency and fidelity

4. Collaborative Environment
* Seamless shared multi-user and multi-device scenarios
* Support for mixed and dynamic user and device configurations e.g., desktop, mobile, and immersive devices
* World-agnostic user identification and data authentication (e.g., SSO)

Linking to a virtual world as an endpoint can provide a unified API to expose standard concepts such as users, views, and spatial content in a unified container. The endpoint API should include functions to join, view, and preview the world in a standard browser/user agent for a given user. Modern web app techniques, including adaptive and responsive frameworks that react to device and network requirements, can be applied to create widely accessible rich user experiences in the browser.

We can see examples of this pattern across the Web today in Single-Page Applications (SPAs) and Web Apps, such as Google Docs, where the user, state, and history are all identified on the URL. So, what information would be essential to represent on a metaverse experience endpoint? Our investigation into use cases will help us enumerate requirements.

## Initial Requirements for Web of Worlds

* We propose the following requirements for the Web of Worlds model:
* Composition of world experiences from multiple assets and endpoints
* Ability to jump to predefined viewpoints in worlds
* Creation and sharing of new viewpoints
* Provision of a preview of the experience before entering
* Experience consistency, e.g., in view and navigation parameters, units, physics
* Security, e.g., protection against Man in the Middle attacks

## Opportunity: Building on Web API on the modern web

To meet these requirements, we propose the following strategy:

* **Build on existing Web and HTTP/HTTPS stack and standards**
  * Providing a single URL endpoint for each addressable world
  * E.g. “http://example.com/superverse/395844”
    
* Enable opening the URL in a user agent to join the world as an interactive experience
  * Automatic user ID controlled join/rejoin management
  * Web-App controlled IO/data/pixel flow
    * e.g., Local data vs remote rendering or even spart streaming
  * Existing users & views should be addressable
    * e.g., “superverse/395844/user/983”

* Optionally open the URL in a user agent to preview the world
  * No additional user created, but user-based authorization needed
  * Web-App controlled IO/data/pixel flow
  * Existing users/views should be addressable

* Optionally expose scene state as model data
  * Including external links, using multiple asset standards, e.g., X3D, USD, glTF

# API Proposals

![objects](specification/figures/objects.svg)

## Open Spatial World API

[OpenSpatialWorld API](specification/OpenSpatialWorld)

## Open Spatial Asset API

[OpenSpatialAsset API](specification/OpenSpatialAsset)

# Implementations

## Open Spatial World API

| Name | License | Level | Asset Reference | Structure Provisioning |  
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
| threedy industrial Metaverse Use-Case | [threedy.space/msf/60394sdf6](http://threedy.space/ms/60394sdf6) | 5 | 

# Standardization
