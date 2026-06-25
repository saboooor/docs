# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/velocity-setup

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/velocity-setup.md).

First, you need to put DimensionsVelocity.jar inside the plugins folder in your proxy.

Now, you need to open **./plugins/dimensionsvelocity/config.toml** and set the following to whatever suits your needs

Copy

```
config-version: "1.0.0" # This is important, it must be included BUT NOT MODIFIED
fallbackServer: "<your main server where you want players to travel if the portal cannot find a destination portal>"
Portals: [
    "<portalName>-><server>",
#   "examplePortal->serverOne",
#   "otherPortal->netherServer",
#   "<portalName>-><serverName>", #This will teleport the player to the specified server when the specified portal is used, and if the portal used is in <serverName> then the player would be teleported in the fallbackServer mentioned in the config
#   "<serverFrom>-><portalName>-><serverName>" #Now this will work like the above but if the portal used was in the <serverFrom> it will ALWAYS teleport to <serverName> no matter what
]
```

The portal name is the file name of the portal in every server and must be the same otherwise the plugin is not going to function properly

Now you need to move to your spigot/paper server to complete the setup

[Spigot/Paper setup](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/spigot-paper-setup)

[PreviousBungee setup](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/bungee-setup) [NextSpigot/Paper setup](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/spigot-paper-setup)

Last updated 2 years ago