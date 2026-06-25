# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/biomes-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/biomes-addon.md).

## 

What does it do?

With biomes addon, you can restrict portals from being used in certain biomes.

## 

How is it configured?

Copy

```
Addon:
  Biomes:
    Allowed: '<input1>'
    DenyMessage: '<input2>'
```

- <input1> = 'all' to disable or list all the allowed biomes you want to allow (seperated with comma (,)) or use 'all, (list all the biomes you want to disabled seperated with comma (,) and each biome starting with (!))'. For example (all, !plains) to allow all biomes apart form plains or another example (plains) to enable only plains
 
- <input2> = any string text you want to be shown to the player if the weather is not suitable
 

[PreviousPermissions addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/permissions-addon) [NextDayLightSensor addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/daylightsensor-addon)

Last updated 3 years ago