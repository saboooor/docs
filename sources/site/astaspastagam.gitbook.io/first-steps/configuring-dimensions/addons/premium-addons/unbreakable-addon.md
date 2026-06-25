# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/unbreakable-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/unbreakable-addon.md).

## 

What does it do?

With Unbreakable addon, you can make a portal indestructible from specific sources such as creeper explosions, or make the portal only breakable by destroying its blocks (and not the inside part of it)

## 

How is it configured?

Copy

```
Addon:
  Unbreakable:
    - '<input>'
```

<input>:

- PLAYER\_INSIDE # player attacks the portal inside (portal entity)
 
- PLAYER #the destroyer was a player (by breaking the blocks)
 
- ENTITY #the destroyer was an entity (creeper by explosion etc)
 
- DISPENSER #a dispenser destroyed the portal (currently dispensers do not break the portal)
 
- PISTON #a piston destroyed the portal
 
- BLOCK\_PHYSICS #a block changed due to block behavior (dirt becomes grass etc)
 

This option is a list. You can add more options by adding a new line and then another **\- <input>**

[PreviousPremium Addons](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons) [NextHubWorld addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/hubworld-addon)

Last updated 3 years ago