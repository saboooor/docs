# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/ignitebyevent-addon-beta

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/ignitebyevent-addon-beta.md).

This wiki is for IgniteByEvent addon v3.0.1-BETA

## 

What does it do?

Portals can now be ignited without only using an item

## 

How is it configured?

Copy

```
Addon:
  IgniteByEvent:
    Enable: true
    Events:
      DropItem:
        #- 'diamond'
        #- 'iron_ingot'
        #- '<item name>'
      EntityDeath:
        #- 'sheep'
        #- 'player'
        #- '<entity type>'
```

[PreviousModelEngine addon (BETA)](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/modelengine-addon-beta) [NextThird party addons](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/third-party-addons)

Last updated 3 years ago