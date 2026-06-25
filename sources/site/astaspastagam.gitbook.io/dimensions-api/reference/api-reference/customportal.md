# Source: https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/customportal

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/dimensions-api/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/customportal.md).

## 

Creating a new portal

You should not create a CustomPortal since it should only be loaded by the [CustomPortalLoader](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/customportal/CustomPortalLoader.html) from the **./plugins/Dimensions/Portals/** directory.

## 

Overriding portal

Addons should not have much control over the CustomPortal that is being loaded since they are supposed to _add_ features to Dimensions and not override them. But there are these methods that you can use to override Dimensions portals without too much work and event cancelling:

- [CustomPortal#setInsideBlockData(BlockData)](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/customportal/CustomPortal.html#setInsideBlockData(org.bukkit.block.data.BlockData))
 
- [PortalGeometry#setCustomGeometry​(CustomPortal, PortalGeometry)](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/completePortal/PortalGeometry.html#setCustomGeometry(me.xxastaspastaxx.dimensions.customportal.CustomPortal,me.xxastaspastaxx.dimensions.completePortal.PortalGeometry))
 

[PreviousAPI Reference](https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference) [NextCompletePortal](https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/completeportal)

Last updated 3 years ago