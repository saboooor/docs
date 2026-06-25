# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/dimensions-configuration

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/dimensions-configuration.md).

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FnZHOfpEDEFnnaUIyafRw%252Fimage.png%3Falt%3Dmedia%26token%3Dd4fa481c-9957-4d34-be92-775240764299&width=768&dpr=3&quality=100&sign=ef9c369f&sv=2)

- checkForUpdatesOnStartup: <default: false> | Set to true if you want everytime your server loads to check for addon updates and installed the new versions that are available.
 
- searchRadius: <default: 128> | Set the distance you want for Dimensions to search for already built portals. This will be used when a player uses a portal and the plugin searches for portals already built and active.
 
- safeSpotSearchRadius: <default: 16> | 16x16 blocks radius that Dimensions will use to search for a safe spot to build a portal.
 
- debugLevel: <dfault: 2> | You can set the level of information that you want to see in your console about Dimensions.
 
 Copy
 
 ```
    DEBUG = 5;
    VERY_LOW = 4;
    LOW = 3;
    MEDIUM = 2;
    HIGH = 1;
    VERY_HIGH = 0;
    ```
 
- enableNetherPortalEffect: <default: true> | Players will see the nether portal effect when they enter a portal.
 
- fallbackWorld: <default: world> | Here you need to enter the name of the world you want to use as a default world. For example if your players play in the world called "survivalWorld" and they use portals to travel arround, then you need to set the default world to "survivalWorld".
 
- configVersion: <x> | Do not change that, that is used for version contol
 
- consumeItems: <default: true> | Toggle if you want items/buckets to not be damaged/consumed when a player tries to ignite a portal.
 
- searchSameAxis: <default: false> | If true, it will search for already existing portals that are built along the same axis
 
- searchSameSize: <default: false> | If true, it will search for already existing portals that are built with the same size
 
- searchFirstClonePortal: <default: true> | If true, it will first search for same size and same axis portals, if not, it will just search using the values above
 
- enableEntitiesTeleport: <default: false> | If true, entities will teleport (teleport delay always applies to them)
 
- updateEveryTick: <default: 7> | This is every how many ticks portals will check for entities nearby in order to teleport them. (This does not apply to players)
 

You can also set the min/max world heights in the config like that:

Copy

```
Worlds:
  <world name>:
    MinHeight: <min Y that you want portals to teleport to>
    MaxHeight: <max Y that you want portals to teleport to>
    Size: <the size of the world as if you were going to change the world border>
```

[PreviousHow does it work?](https://astaspastagam.gitbook.io/first-steps/general-info/how-does-it-work) [NextPortal configuration](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/portal-configuration)

Last updated 3 years ago