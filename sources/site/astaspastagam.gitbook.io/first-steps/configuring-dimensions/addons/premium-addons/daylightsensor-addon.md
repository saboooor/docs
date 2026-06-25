# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/daylightsensor-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/daylightsensor-addon.md).

## 

What does it do?

This addons gives you the ability to make portals only be activatable during a specific time of day (in game).

## 

How is it configured?

Copy

```
Addon:
  DayLightSensor:
    StartAllow: '<input1>'
    StopAllow: '<input2>'
    DenyMessage: '<input3>'
```

- <input1> = any integer
 
- <input2> = any integer
 
- <input3> = any string text you want to be shown to the player if the time is not in range
 

You can set **StartAllow** to the time you want the portals to start being able to be ignited and you can set **StopAllow** to the time you want the portals to stop being able to be ignited. If you set **StartAllow** to a higher integer than **StopAllow** then the portals will be able to be ignited after X & then before Y the next day.

NOTE: setting the same time to min and max disables the addon

[PreviousBiomes addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/biomes-addon) [NextLimited uses addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/limited-uses-addon)

Last updated 3 years ago