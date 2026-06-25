# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/timed-portals-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/timed-portals-addon.md).

## 

What does it do?

Portals will auto-destruct after a configured time of being lit.

## 

How is it configured?

Copy

```
Addon:
  TimedPortals:
    DestroyAfterMillis: <input1>
    Action: '<input2>'
    Effects: #input3
      - '[millis]->[particle pack]'
```

- input1: any integer above zero (0) that indicates how many milliseconds this portal will be activated before being destroyed
 
- input2: you can use between 'Close' or 'Destroy'. **Close** will just break the portal like you would if you attacked the inside of it and **Destroy** will also remove the frame blocks. You can also add {explode%<integer 0-100>} if you want the portal to explode. The integer after the **%** are the chances of the portal exploding.
 
- input3: here you must list all the effects you want to play (from the [ParticlesAddon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/particles-addon)) and the delay for every effect.
 

Effects Example:

Copy

```
  Effects:
#   - '[milliseconds after ignite]->[particle pack name]'
    - '1000->timer1'
    - '2000->timer1'
    - '3000->timer1'
    - '4000->timer1'
    - '5000->timer2'
    - '5500->timer3'
```

[PreviousLimited uses addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/limited-uses-addon) [NextMessage on use addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/message-on-use-addon)

Last updated 3 years ago