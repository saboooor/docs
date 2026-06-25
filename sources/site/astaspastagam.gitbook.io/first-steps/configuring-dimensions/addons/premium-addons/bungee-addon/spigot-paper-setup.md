# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/spigot-paper-setup

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/spigot-paper-setup.md).

Now we are done with the the proxy, we move to our servers

You have to do this for your every server that you want dimensions to teleport between servers so you can make one and copy paste to the rest.

Dimensions & BungeeAddon MUST be installed in order for the plugin to work.

For every portal you create, you need to enable the bungee feature from the config like its shown below

Copy

```
  Bungee:
    Enable: true
    DestWorld: 'world' #DestWorld is the default world that the plugin will travel to (unless it has been linked to another portal in another world)
```

And you are done. Now when you use portals they will send you to the server that you set in the Dimesions Proxy config and the plugin will send the players to the world that you specified in each portal config.

[PreviousVelocity setup](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/velocity-setup) [NextModelEngine addon (BETA)](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/modelengine-addon-beta)

Last updated 3 years ago