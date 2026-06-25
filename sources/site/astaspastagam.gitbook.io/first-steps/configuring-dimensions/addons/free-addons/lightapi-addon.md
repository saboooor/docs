# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/lightapi-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/lightapi-addon.md).

## 

What does it do?

Portals now emit block light

Requires [LightAPI](https://www.spigotmc.org/resources/lightapi.4510/) 5.3.0

After the recent paper update, LightAPI requires the following settings in order to work

Copy

```
enable-compatibility-mode: true
force-enable-legacy: true
```

Using these settings may impact server performance

## 

How is it configured?

Copy

```
Addon:
    LightAPI:
        Level: <input>
```

Level can be 0-15. Recommended light level = 10

### 

Portal without light vs Portal with light

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FHI4E0lgSecde6TguBibB%252Fimage.png%3Falt%3Dmedia%26token%3D1b1267ea-1ab8-4df5-9444-0e8d78d1fa32&width=300&dpr=3&quality=100&sign=b7c79e4c&sv=2)![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252Fz61jd8kBNbbHuXSVZBR7%252Fimage.png%3Falt%3Dmedia%26token%3D8ee18566-9f63-4acc-9ee5-282222eb2eb7&width=300&dpr=3&quality=100&sign=54ecbae3&sv=2)

[PreviousForceLink addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/forcelink-addon) [NextPremium Addons](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons)

Last updated 3 years ago