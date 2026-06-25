# Source: https://astaspastagam.gitbook.io/dimensions-api/creating-an-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/dimensions-api/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/dimensions-api/creating-an-addon.md).

[Source code](https://github.com/xXastaspastaXx/Dimensions3) & [Javadocs](https://astaspasta.alwaysdata.net/javadocs)

## 

Main class

Your main class should extend [DimensionsAddon](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/addons/DimensionsAddon.html)

If you want to use the [Dimensions events](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/events/package-summary.html) then your class must also implement [Listener](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/event/Listener.html)

## 

META-INF

When you are done coding, you have to let Dimensions know about the addon otherwise its not going to load it.

You need to create a few folders and files inside our **src** folder.

Copy

```
src
└───main
    └───java
        └───META-INF
            └───services
```

Inside the **services** folder you need to create a new file named:

Copy

```
me.xxastaspastaxx.dimensions.addons.DimensionsAddon
```

Finally, inside the file, enter the path to your main class as you would with **plugin.yml**

This part is required by [ServiceLoader](https://docs.oracle.com/javase/8/docs/api/java/util/ServiceLoader.html) in order to load the addons properly

[PreviousSetting up](https://astaspastagam.gitbook.io/dimensions-api) [NextExample Addon](https://astaspastagam.gitbook.io/dimensions-api/example-addon)

Last updated 3 years ago