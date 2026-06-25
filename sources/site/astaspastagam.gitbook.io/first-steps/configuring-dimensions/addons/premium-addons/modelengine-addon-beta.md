# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/modelengine-addon-beta

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/modelengine-addon-beta.md).

The addon is in BETA stages. Stuff will be added/removed in almost every update

## 

What does it do?

This addon allows you to summon entities with custom models inside the portal

Requires [ModelEngine](https://www.spigotmc.org/resources/conxeptworks-model-engine%E2%80%94ultimate-custom-entity-model-manager-1-16-5-1-19-2.79477/) 2.5.3

**I**f you reload the server and there are spawned models, the models will stay there and won't be removable (unless you use commands to force remove them)

## 

How is it configured?

Copy

```
Addon:
  ModelEngine: #This list will run for every portal entity inside the portal. so when you check (%y%==%minY%) you check if the model will spawn at the bottom of the portal
    # - '<boolean>;<modelName>;<x>,<y>,<z>'
    # Example 1: spawn kindletronjr model inside the outline of the portal
    # - '(%y%==%minY% || %y%==%maxY%) || ((%x%==%minX% || %x%==%maxX%) && (%z%==%minZ% || %z%==%maxZ%));kindletronjr;%x%,%y%,%z%'
    # Example 2: Spawn kindletronjr at the center of the portal
    # - 'once;kindletronjr;%centerX%,%centerY%,%centerZ%'
```

You can use the keyword 'once' in order to only summon the model once at the specified location.

You can use 'DEBBUGER' to debug the first argument

You can use simple mathematical operations for the spawn location

[PreviousSpigot/Paper setup](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/spigot-paper-setup) [NextIgniteByEvent addon (BETA)](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/ignitebyevent-addon-beta)

Last updated 3 years ago