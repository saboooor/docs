# Source: https://astaspastagam.gitbook.io/first-steps/general-info/worlds-dimensions

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/general-info/worlds-dimensions.md).

Worlds or dimensions (however you want to call them) can be either imported or generated.

If you don't have a world you will need a world generation plugin such as [Multiverse-Core](https://www.spigotmc.org/resources/multiverse-core.390/) or [MyWorlds](https://www.spigotmc.org/resources/myworlds.39594/)

Now, if you already have a world generated and you want to use that, you can put the world folder in your root server directory (where the rest of your worlds are and the spigot.jar or server.properties are) and use the name of the folder as the world in the portal config like that:

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FZtE6fDXVtmqWapjp80Sa%252Fimage.png%3Falt%3Dmedia%26token%3D88401a94-edab-455f-a919-4516966dc3ff&width=768&dpr=3&quality=100&sign=f3486373&sv=2)

In the **./plugins/Dimensions/config.yml** you can set the following:

Copy

```
Worlds:
  <world name>:
    MinHeight: <min Y that you want portals to teleport to>
    MaxHeight: <max Y that you want portals to teleport to>
    Size: <the size of the world as if you were going to change the world border>
```

The min/max option is to set the min/max Y that portals will spawn (when building exit portals)

If the size is not set, then it grabs the world border's size and it's used to calculate the world ratio. (more info below)

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FFCxl7FXPuI3m4rszewFO%252Fimage.png%3Falt%3Dmedia%26token%3D35a3d0d6-0c39-4f77-9631-7d5eb1806d02&width=768&dpr=3&quality=100&sign=c6a02f02&sv=2)

[PreviousCommands](https://astaspastagam.gitbook.io/first-steps/commands) [NextHow does it work?](https://astaspastagam.gitbook.io/first-steps/general-info/how-does-it-work)

Last updated 3 years ago