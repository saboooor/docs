# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/hubworld-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/hubworld-addon.md).

## 

What does it do?

Hub world allows you to set a world as a "hub" for a specific portal. Doing so will give you the chance to set up a nice little spawn that every player can get to from any location on the map by building a portal. Using a portal to teleport to the hub and using the portal from the hub again, will teleport them to the last portal they used.

## 

How is it configured?

Copy

```
Addon:
  Hub:
    World: '<input1>'
    Portals:
      List: [] #<input2>
        # - world,x,y,z
      Mode: <input3>
      
  
```

<input1> = 'false' to disable it (or remove the line) or the world that you want to behave as a hub (usually the default world OR the portal world)

<input2> = If input1 is not 'false' then the portals list does not work. In this list you can put all the portal locations you want to set as portal hubs. If a portal is broken, its not removed from here. If ALL hub portals are broken, then the returning portals of players are lost. You dont have to manually input all the portal locations here, you can use the **/dim addHub** command instead (while looking at a portal)

<input3> = 'random' to select a random portal from the list every time the player must be teleported to a hub portal, or 'firstToLast' to teleport to the first portal (from the list) that is lit at the moment of the player teleporting

[PreviousUnbreakable addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/unbreakable-addon) [NextRandom location addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/random-location-addon)

Last updated 3 years ago