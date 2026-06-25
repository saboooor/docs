# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/limited-uses-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/limited-uses-addon.md).

## 

What does it do?

The portal can be set to auto-destruct after being used too many times.

## 

How is it configured?

Copy

```
Addon:
  LimitedUses:
    MaxUses: <input1>
    Action: '<input2>'
```

- input1: any integer above zero (0) that indicates how many times this portal can be used by any player in order to be destroyed
 
- input2: you can use between 'Close' or 'Destroy'. **Close** will just break the portal like you would if you attacked the inside of it and **Destroy** will also remove the frame blocks. You can also add {explode%<integer 0-100>} if you want the portal to explode. The integer after the **%** are the chances of the portal exploding.
 

[PreviousDayLightSensor addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/daylightsensor-addon) [NextTimed portals addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/timed-portals-addon)

Last updated 3 years ago