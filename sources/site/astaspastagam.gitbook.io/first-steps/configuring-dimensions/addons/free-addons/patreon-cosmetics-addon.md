# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/patreon-cosmetics-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/patreon-cosmetics-addon.md).

## 

What does it do?

The addon gives cosmetic benefits to the users who have donated/subscribed to patreon

## 

How is it configured?

The addon does not need to be configured, its plug & play. Players that have linked their minecraft & patreon accounts in the Dimensions website, will be able to use their benefits in the server.

The server owners are not obligated to use the addon but it would support the plugin if they did and as a Thank you they get to use the benefits in their own server. They can do so by setting the following values in the config.yml

Copy

```
CosmeticsAddon:
    PlayerUUID: <your uuid>
    IgnitePortal: <cosmetic>
    DestroyPortal: <cosmetic>
    UsePortal: <cosmetic>
```

Currently there are only 5 comsetic options. But many more are coming very soon

- NOTHING - disables the effects
 
- FINAL\_SPARK | use, destroy, ignite
 
- FILLING\_THE\_VOID | tick, use, destroy, ignite
 
- HEART\_SEEKER | tick, use, destroy, ignite
 
- HUNGRY\_HOUNDS | tick, use, destroy, ignite
 
- GLOWING\_AURA | tick
 
- ANGRY\_LLAMA | tick
 
- EXPLOSIONS | destroy, use
 
- LIL\_RING | tick
 

The words after the effects have the following meaning:

- use = you can put it at UsePortal
 
- ignite = you can put it at IgnitePortal
 
- destroy = you can put it at DestroyPortal
 
- tick = you can put it at PortalTick
 

[PreviousWorld guard flags addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/world-guard-flags-addon) [NextHorizontal portals addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/horizontal-portals-addon)

Last updated 3 years ago