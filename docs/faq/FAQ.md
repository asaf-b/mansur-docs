# Frequently Asked Questions

### Installation
- [I installed Mansur-Rig, and I don't see the menu in Maya](#i-installed-mansur-rig-and-i-dont-see-the-menu-in-maya)
- [I'm a freelance rigging artist using Mansur-Rig. do my clients require Mansur-Rig?](#im-a-freelance-rigging-artist-using-mansur-rig-do-my-clients-require-mansur-rig)
- [Do animators require Mansur-Rig?](#do-animators-require-mansur-rig)
- [After extracting the skeleton, do I still need Mansur-Rig?](#after-extracting-the-skeleton-do-i-still-need-mansur-rig)
- [Can I install Mansur-Rig in other softwares other then Maya?](#can-i-install-mansur-rig-in-other-softwares-other-then-maya)

### Pricing/Subscriptions
- [What is the key difference between the *Gold* and *Silver* subscription plans?](#what-is-the-key-difference-between-the-gold-and-silver-subscription-plans)
- [Can  sell rigs created using Mansur-Rig?](#can-sell-rigs-created-using-mansur-rig)
- [Is there an option to get an annual subscription?](#is-there-an-option-to-get-an-annual-subscription)
- [Does Mansur-Rig offer student license discounts?](#does-mansur-rig-offer-student-license-discounts)

### Custom Rigging
- Can I add manual steps to Mansur-Rig's build?
- Can I write my own modules?
- Can I use Mansur-Rig's node-library without block?

### License Management
- [I want to use Mansur-Rig in a studio, and I need multiple licenses for my users. What do I do?](#i-want-to-use-mansur-rig-in-a-studio-and-i-need-multiple-licenses-for-my-users-what-do-i-do)
- [I want to test Mansur-Rig for studio use, and m Trial is expired. what do I do?](#i-want-to-test-mansur-rig-for-studio-use-and-my-trial-is-expired-what-do-i-do)
- [I use Mansur-Rig in a studio environment, do I need to credit it?](#i-use-mansur-rig-in-a-studio-environment-do-i-need-to-credit-it)

### Development
- [Is Mansur-Rig maintained?](#is-mansur-rig-maintained)
- [Where can I track Mansur-Rig's Development?](#where-can-i-track-mansur-rigs-development)
- [I have a bug to report, where can I do that?](#i-have-a-bug-to-report-where-can-i-do-that)
- [I have a feature request, where can I send it to?](#i-have-a-feature-request-where-can-i-send-it-to)

<hr>

### Installation [Answers]

#### I installed Mansur-Rig, and I don't see the menu in Maya
> * First, make sure the Maya version in question is within Mansur-Rig's supported versions, and that you are using a supported platform: <br>[*System-Requirements*](../../userGuides/System-Requirements/)
> * If so, make sure PyMel is installed within the Maya version you are using: <br>[*2022 & 2023*](../../userGuides/System-Requirements/#maya-2022-2023-requirements) <br>[*2024*](../../userGuides/System-Requirements/#maya-2024-requirements)
> * Try to uninstall, then use the [*manual installation*](../../userGuides/installation/#manual-installation) instead. 
> * If non if the above make a difference, please send a support ticket to <br>**support@mansur-rig.com** <br>with as much information possible.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### I'm a freelance rigging artist using Mansur-Rig. do my clients require Mansur-Rig?
> Yes.
> Mansur-Rig is based on a dedicated custom C++ node library, that is the heart of it's operation.
> In order for the Rigs created using Mansur-Rig to run, this solver-library is required. Without it, it won't function.
> Moreover, Mansur-Rig's solvers will only function in case Mansur-Rig is activated using a valid license.
> So, your clients will require the installation of Mansur-Rig, as well as a valid license to activate it within Maya for them to be able to use the rig you created using Mansur-Rig.
> With that said, in case your clients only need to animate using the rig (not build it), they will only require the lower tier *Silver* license.
>
> It is also important to note that in case your clients only need to use Mansur-Rig's extracted skeleton for a game-engine for example- they do not require Mansur-Rig at all.
> Mansur-Rig is only required to build/use puppets within Maya. Once the sekeleton/animated-skeleton is extracted, Mansur-Rig is no longer required.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Do animators require Mansur-Rig?
> Yes.
> Mansur-Rig is required to build/use puppets created using Mansur-Rig within Maya.
> With that said, Animators only require the lower tier *Silver* license.

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


### Pricing/Subscriptions [Answers]

#### What is the key difference between the *Gold* and *Silver* subscription plans?
> The key difference is the fact the the *Gold* subscription is targeted for Riggers, while the *Silver* subscription is targeted for Animators.
>
> * The *Gold* license has no restrictions. All actions/tools/nodes within Mansur-Rig are open for *Gold* subscribers.
> * The *Silver* license is a 'Read-Only' subscription. Meaning that all *Build* actions, or *Change* actions are not avilable. Although all animation related tools are avilable. This license is designed for Animators who only need to **use** rigs created using Mansur-Rig, rather then build/change them.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Can  sell rigs created using Mansur-Rig?
> Yes, Absulotly.  
> Anyone is free to sell rigs created using Mansur-Rig, without any restrictions, and without any prior approval, and at any price.  
> Also, there is no requirement to credit Mansur-Rig. Although that will help support Mansur-Rig and will be appreciated.  
> <br>
> With that said, remember that Mansur-Rig is required (installation and license) in order for the rigs your are selling to function.  
> So anyone you sell your rigs to, will require to install and validate Mansur-Rig.  

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Is there an option to get an annual subscription?
> Not currently.  
> It is on the road-map, but there is no ETA at the moment.  
> <br>
> Note: An exception can be made for studio teams, please contact us at<br>**support@mansur-rig.com**<br> if that is your case and you are interested.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### Does Mansur-Rig offer student license discounts?
> Unfortunately, not currently.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

### License Management [Answers]

#### I want to use Mansur-Rig in a studio, and I need multiple licenses for my users. What do I do?
> No problem at all.  
> Mansur-Rig has an enterprise-level license management system.  
> Using [*Mansur-Rig's Web-App*](https://app.mansur-rig.com/) you can easily acquire multiple licenses (of both *Gold* and *Silver*) and assign these licenses to your users.  
> Your users will only be able to log-in and log-out using these assigned licenses, while you as the licenses owner will be able to manage them.  
> Assigned licenses can always be retreived and re-used for changing users, and the amount of licenses you own can always be changed according to you needs.  
> Here is a [video guide to the license management system](https://youtu.be/wMmrZVSf9tk?si=9Ildam5eX_rwKbbu)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### I use Mansur-Rig in a studio environment, do I need to credit it?
> No.  
> Although that will help support Mansur-Rig and will be very appreciated.

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### I want to test Mansur-Rig for studio use, and my Trial is expired. what do I do?
> Please contact us at<br>**support@mansur-rig.com**<br> and we will gladly support your needs.

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
> You can also send a support ticket to<br>**support@mansur-rig.com**  
> In case your report was reproduced successfully, it will be logged to our [*Development Board*](https://trello.com/b/dBw02z9a/mansur-rig-development)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>

#### I have a feature request, where can I send it to?
> First, you can try our live support at our [*Discord Server*](https://discord.gg/nXfy3Rh5y6)  
> You can also send a feature request to<br>**support@mansur-rig.com**  
> In case your feature request was accepted, it will be logged to our [*Development Board*](https://trello.com/b/dBw02z9a/mansur-rig-development)

<a href="#top">↑ Back to top ↑</a>
<br>
<br>