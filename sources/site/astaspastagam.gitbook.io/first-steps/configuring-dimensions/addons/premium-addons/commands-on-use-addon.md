# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/commands-on-use-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/commands-on-use-addon.md).

## 

What does it do?

The addon gives you the ability to execute commands when a player uses the portal

## 

How is it configured?

Copy

```
Addon:
  Commands:
    - '<input1>;<input2>;<input3>'
```

- input1: who is going to execute the command (values= **player** or **console**)
 
- input2: pre-conditions for the command to be executed. For example `((%destinationWorld%==world6 && %entity%==astaspasta) || %portal%==samplePortal) && %zAxis%`. `true` can be used if you want the command to run anyway
 
- input3: the command to execute.
 

For example `tell %entity% you used a zAxis portal and its name is samplePortal or your name is astaspasta and you came from world6`

If you plan to override the teleport of Dimensions (for example for a random location command) then It's recommended that you add the following to your portal config. (This addon option is provided by the CommandsOnUse addon)

Copy

```
Addon:
  DisableTeleport: true
```

Copy

```
Placeholders:
%portal% - Portal display name
%name% - Portal name
%entity% - Player name/Entity Type
%entityID% - Player UUID/Entity ID

%destinationWorld% - Destination world
%destinationX% - Destination X
%destinationY% - Destination Y
%destinationZ% - Destination Z

%originalWorld% - Original world
%originalX% - Original X
%originalY% - Original Y
%originalZ% - Original Z

%zAxis% - True if portal is Facing the X Axis (aka portal is build along the Z Axis

The CommandsOnUse Addon also supports PlaceholderAPI placeholders
```

[PreviousBetter portals addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/better-portals-addon) [NextStylish portals addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/stylish-portals-addon)

Last updated 3 years ago