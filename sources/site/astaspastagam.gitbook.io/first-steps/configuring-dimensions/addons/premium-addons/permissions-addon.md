# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/permissions-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/permissions-addon.md).

## 

What does it do?

You can set permissions for each portal using this addon. Players that do not have permissions will not be able to ignite or use the portal.

## 

How is it configured?

Copy

```
Addon:
  Permission:
    Node: '<input1>'
    DenyMessage: '<input2>'
```

- <input1> = 'none' to disable or any string text you want to be the permission (e.x dimensions.useportal.samplePortal)
 
- <input2> = any string text you want to be shown to the player if they dont have permission
 

[PreviousRandom location addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/random-location-addon) [NextBiomes addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/biomes-addon)

Last updated 3 years ago