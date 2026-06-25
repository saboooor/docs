# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/bungee-setup

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/bungee-setup.md).

First, you need to put DimensionsBungee.jar inside the plugins folder in your proxy.

Now, you need to open **./plugins/DimensionsBungee/config.yml** and set the following to whatever suits your needs

Copy

```
fallbackServer: <your main server where you want players to travel if the portal cannot find a destination portal>
Portals:
 - '<portalName>-><server>'
#- 'examplePortal->serverOne'
#- 'otherPortal->netherServer'
#- '<portalName>-><serverName>' #This will teleport the player to the specified server when the specified portal is used, and if the portal used is in <serverName> then the player would be teleported in the fallbackServer mentioned in the config
#- '<serverFrom>-><portalName>-><serverName>' #Now this will work like the above but if the portal used was in the <serverFrom> it will ALWAYS teleport to <serverName> no matter what
```

The portal name is the file name of the portal in every server and must be the same otherwise the plugin is not going to function properly

Now you need to move to your spigot/paper server to complete the setup

[Spigot/Paper setup](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/spigot-paper-setup)

[PreviousBungee addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon) [NextVelocity setup](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/velocity-setup)

Last updated 3 years ago