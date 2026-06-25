# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/stylish-portals-addon

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/stylish-portals-addon.md).

## 

What does it do?

Gives you the ability to make portals that are not made from a specific block type using different patterns

You can set the pattern for the portal in the portal config for the top of the portal, the left side, the right side and the bottom.

## 

How is it configured?

Example configuration:

Copy

```
Addon:
  StylishPortal:
    FrameStyle:
      - 'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]|minecraft:waxed_cut_copper|minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]'
      - 'minecraft:waxed_cut_copper_stairs[facing=west,half=top,shape=straight,waterlogged=false]|minecraft:waxed_cut_copper_stairs[facing=west,half=bottom,shape=straight,waterlogged=false]\minecraft:waxed_cut_copper_stairs[facing=west,half=top,shape=straight,waterlogged=false]'
      - 'minecraft:waxed_cut_copper_stairs[facing=east,half=top,shape=straight,waterlogged=false]|minecraft:waxed_cut_copper_stairs[facing=east,half=bottom,shape=straight,waterlogged=false]\minecraft:waxed_cut_copper_stairs[facing=east,half=top,shape=straight,waterlogged=false]'
      - 'minecraft:waxed_cut_copper_slab[type=top,waterlogged=false]|minecraft:waxed_cut_copper|minecraft:waxed_cut_copper_slab[type=top,waterlogged=false]'
```

Using this in your portal will result in a portal like this

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FQW9wQJIaxu9E3DLLodOV%252FScreenshot_1.png%3Falt%3Dmedia%26token%3D044f060d-12c1-4b62-b8dd-31e7360cd620&width=768&dpr=3&quality=100&sign=547c4129&sv=2)

very cool yes yes

If you dont care about a specific block what it's going to be built with, then you can use the **dimensions:placeholderblock**

dimensions:placeholderblock = dimensions:placeholderblock\[all,!air,!cave\_air\]

Usage: dimensions:placeholderblock\[<material>,<material>,<material>\]

Usage: dimensions:placeholderblock\[all,!<material>,!<material>,!<material>\]

> What is this long spaghetti?

The portal style is built from a list of 4 strings, TOP, RIGHT SIDE, LEFT SIDE, BOTTOM

IMPORTANT: The right and left side pattern starts from the top side of the portal excluding the first block and end at the bottom excluding the last block

Each line consists of different PATTERNS that the portal must be built in order to be considered a portal and each pattern is separated with the symbol |

If there is only one pattern (no |) then the whole part of the portal must be that pattern

If there are two or more patterns then the portal MUST START with the first pattern and MUST END with the last. The rest of the portal must be a repeat of the second & third & ... & _last-1_ patterns.

In the example above, we have the roof of our portal starting with a copper slab (bottom slab) then a repeat of copper blocks and then the portal must end with a copper slab (bottom slab).

Each pattern can either have a single block or a series of blocks separated with the "\\" symbol.

For example in our right side (second line) our pattern starts with the stairs looking down and then its a repeat of stairs looking up then down then up then down (THE PATTERN MUST BE COMPLETE NO MATTER HOW MANY TIMES TO BE CONSIDERED A PORTAL)

> How do i create my own style?

Well, for now its a kinda long process and goes as follows:

First you connect to your server (with this addon installed) and build the portal you want to have IN THE X AXIS and when you look at the portal you have to be looking NORTH. (that is to make your life easy)

We will be making the portal above as an example

Now we start with the top part of the bottom.

And we look at the TOP LEFT block (like the screenshot below) and run `/dim blockdata`. Now a message that says click me appears and you click on it to copy the block data to your clipboard and now we move to the portal config to paste it on the first line and we currently have

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FDh8qYkuwa4MvF5xhabfJ%252FScreenshot_2.png%3Falt%3Dmedia%26token%3De8642d63-0050-43c9-81ee-cd8e701c9d7e&width=768&dpr=3&quality=100&sign=60220b20&sv=2)

Copy

```
Addon:
  StylishPortal:
    - 'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]'
    - ''
    - ''
    - ''
```

and then we want the rest of the portal to be a copper block until the end so we add a new pattern (with one block).

We go to the next wall and run the command `/dim blockdata` again and get the block data and we result to:

Copy

```
Addon:
  StylishPortal:
    - 'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]|minecraft:waxed_cut_copper'
    - ''
    - ''
    - ''
```

Now we also want to end with a copper slab so we add another pattern to the end and we end up with

Copy

```
Addon:
  StylishPortal:
    - 'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]|minecraft:waxed_cut_copper|'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]'
    - ''
    - ''
    - ''
```

GREAT! You just created a style for the top of your portal.

For the bottom we do the exact same thing. If you want the exact same style as the top we can just copy and paste the roof patterns so we come with

Copy

```
Addon:
  StylishPortal:
    - 'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]|minecraft:waxed_cut_copper|'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]'
    - ''
    - ''
    - 'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]|minecraft:waxed_cut_copper|'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]'
```

Now for the side we will look at the TOP RIGHT block BELLOW the top part of the portal (see screenshot below)

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FFMDGphDhGd7J3A7ySVKU%252FScreenshot_3.png%3Falt%3Dmedia%26token%3Dc9f888ed-1bbe-4f0e-accb-5b04c6b4f009&width=768&dpr=3&quality=100&sign=51bf5766&sv=2)

The way we do it is so players can make bigger portals without wasting MORE blocks so we will have a down-facing staircase and a pattern of two stairs (one up, one down).

So we will have a starting pattern of a stair looking down. and then a repeating pattern of two (one up, one down).

So we add to the second line which corresponds to the RIGHT side of the portal starting from top (exluding the first/roof block)

`minecraft:waxed_cut_copper_stairs[facing=west,half=top,shape=straight,waterlogged=false]`

which is the starting pattern and then we add `|` to clarify that is the next _to be checked_ pattern which will be repeated to the end of the portal (unless we add a third pattern using the `|` symbol) and then we add

`minecraft:waxed_cut_copper_stairs[facing=west,half=bottom,shape=straight,waterlogged=false]`

as the first block in our new pattern, then we add `\` to clarify that there is a block after the previous that must exist and then we add

`minecraft:waxed_cut_copper_stairs[facing=west,half=top,shape=straight,waterlogged=false]`

which is the block we want to use. We also want the same pattern for the left side of our portal so we copy and paste it on the 3rd line changing the west to east and we end up with

Copy

```
Addon:
  StylishPortal:
    - 'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]|minecraft:waxed_cut_copper|'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]'
    - 'minecraft:waxed_cut_copper_stairs[facing=west,half=top,shape=straight,waterlogged=false]|minecraft:waxed_cut_copper_stairs[facing=west,half=bottom,shape=straight,waterlogged=false]\minecraft:waxed_cut_copper_stairs[facing=west,half=top,shape=straight,waterlogged=false]'
    - 'minecraft:waxed_cut_copper_stairs[facing=east,half=top,shape=straight,waterlogged=false]|minecraft:waxed_cut_copper_stairs[facing=east,half=bottom,shape=straight,waterlogged=false]\minecraft:waxed_cut_copper_stairs[facing=east,half=top,shape=straight,waterlogged=false]'
    - 'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]|minecraft:waxed_cut_copper|'minecraft:waxed_cut_copper_slab[type=bottom,waterlogged=false]'
```

Its a very long text, very long instructions, but after you do it once, it's not that difficult

[PreviousCommands on use addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/commands-on-use-addon) [NextParticles addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/particles-addon)

Last updated 3 years ago