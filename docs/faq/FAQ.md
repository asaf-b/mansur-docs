# Frequently Asked Questions

### Pricing/Subscriptions
- [Is Mansur-Rig free to use?](#is-mansur-rig-free-to-use)
- [Can I sell rigs created using Mansur-Rig?](#can-i-sell-rigs-created-using-mansur-rig)

### Installation
- [How do I install Mansur-Rig?](#how-do-i-install-mansur-rig)
- [I installed Mansur-Rig, and I don't see the menu in Maya](#i-installed-mansur-rig-and-i-dont-see-the-menu-in-maya)
- [I'm a freelance rigging artist using Mansur-Rig. do my clients require Mansur-Rig?](#im-a-freelance-rigging-artist-using-mansur-rig-do-my-clients-require-mansur-rig)
- [Do animators require Mansur-Rig?](#do-animators-require-mansur-rig)
- [After extracting the skeleton, do I still need Mansur-Rig?](#after-extracting-the-skeleton-do-i-still-need-mansur-rig)
- [Can I install Mansur-Rig in other softwares other then Maya?](#can-i-install-mansur-rig-in-other-softwares-other-then-maya)
- [Can I use Mansur-Rig without an internet conection?](#can-i-use-mansur-rig-without-an-internet-conection)

### Compatibility
- [Is Mansur-Rig Game-Engine compatible?](#is-mansur-rig-game-engine-compatible)
- [Is Mansur-Rig joint based?](#is-mansur-rig-joint-based)
- [Can I use Mansur-Rig in combination with another Rig-Builder/manual-rig?](#can-i-use-mansur-rig-in-combination-with-another-rig-buildermanual-rig)
- [I'm using a custom pipeline, and picker images don't load. Can I specify a static location for picker images?](#im-using-a-custom-pipeline-and-picker-images-dont-load-can-i-specify-a-static-location-for-picker-images)
- [Is there an easy way to extract animations from Mansur-Rig to FBX?](#is-there-an-easy-way-to-extract-animations-from-mansur-rig-to-fbx)
- [Can I incorporate Motion-Capture (MOCAP) with Mansur-Rig?](#can-i-incorporate-motion-capture-mocap-with-mansur-rig)

### General
- [Does Mansur-Rig auto skin?](#does-mansur-rig-auto-skin)
- [Can I use Mansur-Rig to create Facial-Rigs?](#can-i-use-mansur-rig-to-create-facial-rigs)
- [What's the difference between Mansur-Rig and other rig-builders?](#whats-the-difference-between-mansur-rig-and-other-rig-builders)
- [Where can I get support?](#where-can-i-get-support)

### Custom Rigging
- [Can I add manual steps to Mansur-Rig's build?](#can-i-add-manual-steps-to-mansur-rigs-build)
- [Can I run Mansur-Rig using code instead of the UI?](##can-i-run-mansur-rig-using-code-instead-of-the-ui)

### Credits
- [I use Mansur-Rig in a studio environment, do I need to credit it?](#i-use-mansur-rig-in-a-studio-environment-do-i-need-to-credit-it)

### Development
- [Is Mansur-Rig maintained?](#is-mansur-rig-maintained)
- [Where can I track Mansur-Rig's Development?](#where-can-i-track-mansur-rigs-development)
- [I have a bug to report, where can I do that?](#i-have-a-bug-to-report-where-can-i-do-that)
- [I have a feature request, where can I send it to?](#i-have-a-feature-request-where-can-i-send-it-to)

<hr>

### Pricing [Answers]

#### Is Mansur-Rig free to use?
> Yes. Mansur-Rig is 100% free to use. For both personal and commercial use.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Can I sell rigs created using Mansur-Rig?
> Yes, absolutely.  
> Anyone is free to sell rigs created using Mansur-Rig, without any restrictions, and without any prior approval, and at any price.  
> Also, there is no requirement to credit Mansur-Rig. Although that will help support Mansur-Rig and will be appreciated.  
> <br>
> With that said, remember that Mansur-Rig is required (installation) in order for the rigs your are selling to function.  
> So anyone you sell your rigs to, will require to install Mansur-Rig. 
> Although it is completely free.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

### Installation [Answers]

#### How do I install Mansur-Rig?
> Here is a video guide on how to install and activate Mansur-Rig:  
> [Installation & Activation Tutorial](../userGuides/installation.md)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### I installed Mansur-Rig, and I don't see the menu in Maya
> * First, make sure the Maya version in question is within Mansur-Rig's supported versions, and that you are using a supported platform: <br>[*System-Requirements*](../userGuides/System-Requirements.md)
> * If so, make sure PyMel is installed within the Maya version you are using: <br>[*2022 & 2023*](../userGuides/System-Requirements.md#maya-2022-2023-requirements) <br>[*2024*](../userGuides/System-Requirements.md#maya-2024-requirements)
> * Try to uninstall, then use the [*manual installation*](../userGuides/installation.md#manual-installation) instead. 
> * If non if the above make a difference, please send a support ticket to <br>**hello@mansur-rig.com** <br>with as much information possible.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### I'm a freelance rigging artist using Mansur-Rig. do my clients require Mansur-Rig?
> Yes.  
> Mansur-Rig is based on a dedicated custom C++ node library, that is the heart of it's operation.  
> In order for the Rigs created using Mansur-Rig to run, this solver-library is required. Without it, it won't function.  
> Although Mansur-Rig is free to use.  
> So, your clients will require the installation of Mansur-Rig.
> <br>
> It is also important to note that in case your clients only need to use Mansur-Rig's extracted skeleton for a game-engine for example- they do not require Mansur-Rig at all.  
> Mansur-Rig is only required to build/use puppets within Maya. Once the sekeleton/animated-skeleton is extracted, Mansur-Rig is no longer required.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Do animators require Mansur-Rig?
> Yes.
> Mansur-Rig's installation is required to build/use puppets created using Mansur-Rig within Maya.
> Although it is completely free.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### After extracting the skeleton, do I still need Mansur-Rig?
> No.
> Mansur-Rig is only required to build/use puppets within Maya. Once the sekeleton/animated-skeleton is extracted, Mansur-Rig is no longer required.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Can I install Mansur-Rig in other softwares other then Maya?
> No.  
> Mansur-Rig is a plugin written specifically for Maya. Although the UI is written in Python, it is based on a dedicated custom C++ node library written using Maya's API, hence running it in any other software other then Maya isn't possible.   
> Transforming Mansur-Rig to other softwares isn't possible as well, just for clarity.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Can I use Mansur-Rig without an internet conection?
> Yes. An internet connection is only needed to download the product.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

### Compatibility [Answers]

#### Is Mansur-Rig Game-Engine compatible?
> Yes.  
> Mansur-Rig was designed to support game engines workflows.  
> In case you are using Mansur-Rig with only a Skin-Cluster and Blend-Shape deformers, your rig is 100% Game-Engine compatible.  
> Mansur-Rig created a single joint hierarchy, with an origin top joint, which is the Game-Engine standard.  
> Also, Mansur-Rig contains easy to use tools to extract animations and assets to *FBX* format to enhence Game-Engine workflows.  
> Mansur-Rig contains MOCAP support and easy to use tools in order to incorporate MOCAP into your workflow easily.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Is Mansur-Rig joint based?
> Yes.  
> Mansur-Rig modules were designed to be joint-driven.  
> As creating modules that are joint-based is usually more difficult, especially for facial rigs, Mansur-Rig was designed to be Game-Engine compatible, hence an effort was made to make sure all functionalities are joint-based.  

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Can I use Mansur-Rig in combination with another Rig-Builder/manual-rig?
> Yes, of course.
> You can combine Mansur-Rig with any other technics of your choice.  
> Although Mansur-Rig does not contain pre-defined ways of combining it with other non-native objects, it is completely up to you do choose to do so.  
> You can choose to use manual actions to connect Mansur-Rig with other entities, or you can use Mansur-Rig's [*Custom-Scripts*](../userGuides/Custom-Scripts.md) to automate this workflow.   

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### I'm using a custom pipeline, and picker images don't load. Can I specify a static location for picker images?
> Yes.  
> Simply go to *Mansur-Rig -> Preferences* dialog, move to *Picker* tab within the preferences dialog, and set your centralized picker-imaged path into the *pickerImagesFallbakPath* setting.  
> Click *Save*  
> Now, if a picker image isn't found, this directory will be used as a fallback directory to try and find it.  
> **Note:** please use [this-guide](../userGuides/tutorials/Creating-A-Picker.md#picker-images-naming-convention) for correct naming convention for picker images

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Is there an easy way to extract animations from Mansur-Rig to FBX?
> Yes.  
> Mansur-Rig contains a comprehensive [*Animation-Exporter*](../userGuides/Game-Exporter.md) that allows fast and easy export of assets/animations to *FBX* format.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Can I incorporate Motion-Capture (MOCAP) with Mansur-Rig?
> Yes.  
> Mansur-Rig supports Motion-Capture workflows fully.  
> Here is a [*Guide to Mansur-Rig's Mocap Tools*](../userGuides/Mocap-And-Game-Tools.md)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

### Credits [Answers]

#### I use Mansur-Rig in a studio environment, do I need to credit it?
> No.  
> Although that will help support Mansur-Rig and will be very appreciated.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

### General [Answers]

#### Does Mansur-Rig auto skin?
> No.  
> Mansur-Rig is a puppet-creation tool and offers no skinning tools.  
> Skinning is an essential skill required in order to build any rig, and Mansur-Rig is no exception.  
> If you are only looking for a tool to enhence/automate your skinning workflow, Mansur-Rig is not a good match.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Can I use Mansur-Rig to create Facial-Rigs?
> Absolutely.  
> Mansur-Rig contains both sepecificaly designed Facial-Rigging modules, as well as many more sulotions to create high-end Facial-Rigs.  
> Moreover, Mansur-Rig's Facial-Rigging methods are one of it's best strengths, and all of them are joint-based as well, so they are also Game-Engine compatible.  
> Check out some examples over at our [*Art-Station*](https://www.artstation.com/mansur-rig) profile and our [*You-Tube Channel*](https://www.youtube.com/channel/UCMjNlJjSxIam--3u87oh5PQ)  
> And here is a full tutorial series on [Mansur-Rig's Facial-Rigging](https://www.youtube.com/playlist?list=PLpTYt5H9lICqxf7wCueB6imuRg1MoE5tU)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### What's the difference between Mansur-Rig and other rig-builders?
> * First and foremost, Mansur-Rig's performance is **faster**. It is based on an extensive custom node-library, dedicated to fast performing rigs.  
> * Second, it's ability to be deconstructed will speed-up your workflow tremendously. Instead of building a puppet from pre-defined guides, one-way-steet, it's **one of a kind ability to be decostructed back to guides state** means that your puppet and guides are the same entity.  
> * This in turn means that your **rig building iterations are much faster**. Instead of needing to re-open "guides" file and building again, you simply go back and forth between constructed and decustrected states.  
> * This also means, that **ALL rig information is within one scene**. No longer you need to manage multiple files containing different types of data. Your guides, controls, rig-poses, control shapes, picker information and skin-data are contained within a single Maya scene.  
> * This **unique ability** also allows you to pre-pose your puppet- which is very significant. Instead of being dependent of the Modeling team to deliver a T-Posed model (which isn't optimal), using Mansur-Rig you will be liberated to pre-pose your model, since the skin-data is a part of your rig, instead of being loaded post-construction. The skinning information is preserved in both constructed and deconstructed states, so **you can pose your rig before constrcuting the puppet**. Your animators will feel the difference- it's MASSIVE.  
> * Next, Mansur-Rig's components are to the **highest possible extent of modularity**. Not only you can combine any component with any different one, the components are layered so you can choose the amount of flexibility you provide within your rig based on your performance limitations. You can also connect components using a centralized *spaces* system.
> * Since Mansur-Rig has dual states, **every rig is also a template**. You can use ANY Mansur-Rig's puppet and simply deconstruct it- and just like that you have a guide template. Move components to their new location based on your model, construct, and the puppet will match the original puppet you based you rig on. Of course you can always deconstruct and alter settings/components to your needs.
> * Overall, Mansur-Rig is the single high end One-Stop-Shop for all of your rigging needs. **A production ready proven product, suitable for both offline productions and Game-Engines**.
> * Finally- **completeness**. Mansur-Rig contains many tools for rigging and animation workflows to support it's main behaviour. These tools are a part of the product and don't need to be externaly installed. They are simply there whenever you need them:
> 1. [LOD Tool](../userGuides/LODs-Tool.md)
> 2. [Animation Picker](../userGuides/The-Picker.md)
> 3. [Control Visibility Tool](../userGuides/Control-Visibility-Tool.md)
> 4. [CNS Tool](../userGuides/CNS-Tool.md)
> 5. [Spring Tool](../userGuides/Spring-Tool.md)
> 6. [Spaces/IK-FK Tool](../userGuides/Spaces-IK-FK-Tool.md)
> 7. Facial Mocap Tool
> 8. [Animation Exporter](../userGuides/Game-Exporter.md)
> 9. [Volume-Joints Tool](../userGuides/Volume-Joints.md)
> 10. [Deformation Utilities](../userGuides/Deformation-Utilities.md)
> 11. [MOCAP tools](../userGuides/Mocap-And-Game-Tools.md)
> 12. [Module-Preset Editor](../userGuides/Module-Preset-Editor.md)
> 12. [Dynamic UI Creation Tool](../userGuides/Dynamic-UI-Creator.md)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>


#### Where can I get support?
> In case you are having any issues with your product or your account, here are the ways to get in touch:
>
> * Live-Support at [Mansur-Rig's Discord Server](https://discord.gg/nXfy3Rh5y6)
> * Send an email directly to <b>hello@Mansur-Rig.com</b> 
> * This official [Mansur-Rig documentation page](https://docs.mansur-rig.com/)
> * The official [Mansur-Rig You-Tube Channel](https://www.youtube.com/channel/UCMjNlJjSxIam--3u87oh5PQ)
> * PM using any social media.
> * Any official and unofficial guides/tutorials.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

### Custom Rigging [Answers]

#### Can I add manual steps to Mansur-Rig's build?
> Yes.  
> Please follow this guide to [*Custom-Scripts*](../userGuides/Custom-Scripts.md) in order to add python-scripts to Mansur-Rig's automated build.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Can I run Mansur-Rig using code instead of the UI?
> Yes.  
> Here is a [*Guide To Scripted Builds*](../userGuides/Scripted-Builds.md)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

### Development [Answers]

#### Is Mansur-Rig maintained?
> YES!  
> Mansur-Rig is an ongoing development, and **IT IS HERE TO STAY!**

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Where can I track Mansur-Rig's Development?
> You can follow Mansur-Rig's developement on our [*Development Board*](https://trello.com/b/dBw02z9a/mansur-rig-development)  
> You can also track past development and release notes at the [*Release Notes Page*](../releaseNotes/v2.4.0.md)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### I have a bug to report, where can I do that?
> First, you can try our live support at our [*Discord Server*](https://discord.gg/nXfy3Rh5y6)  
> You can also send a support ticket to<br>**hello@mansur-rig.com**  
> In case your report was reproduced successfully, it will be logged to our [*Development Board*](https://trello.com/b/dBw02z9a/mansur-rig-development)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### I have a feature request, where can I send it to?
> First, you can try our live support at our [*Discord Server*](https://discord.gg/nXfy3Rh5y6)  
> You can also send a feature request to<br>**hello@mansur-rig.com**  
> In case your feature request was accepted, it will be logged to our [*Development Board*](https://trello.com/b/dBw02z9a/mansur-rig-development)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>