# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/dimensions-configuration.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/dimensions-configuration.md).

# Dimensions configuration

!\[\](/files/rXj7lgL921ZpYCT40doZ)

\* checkForUpdatesOnStartup: \\<default: false> | Set to true if you want everytime your server loads to check for addon updates and installed the new versions that are available.
\* searchRadius: \\<default: 128> | Set the distance you want for Dimensions to search for already built portals. This will be used when a player uses a portal and the plugin searches for portals already built and active.
\* safeSpotSearchRadius: \\<default: 16> | 16x16 blocks radius that Dimensions will use to search for a safe spot to build a portal.
\* debugLevel: \\<dfault: 2> | You can set the level of information that you want to see in your console about Dimensions.

 \`\`\`
  DEBUG = 5;
  VERY\_LOW = 4;
  LOW = 3;
  MEDIUM = 2;
  HIGH = 1;
  VERY\_HIGH = 0;
  \`\`\`
\* enableNetherPortalEffect: \\<default: true> | Players will see the nether portal effect when they enter a portal.
\* fallbackWorld: \\<default: world> | Here you need to enter the name of the world you want to use as a default world. For example if your players play in the world called "survivalWorld" and they use portals to travel arround, then you need to set the default world to "survivalWorld".
\* configVersion: \\<x> | Do not change that, that is used for version contol
\* consumeItems: \\<default: true> | Toggle if you want items/buckets to not be damaged/consumed when a player tries to ignite a portal.
\* searchSameAxis: \\<default: false> | If true, it will search for already existing portals that are built along the same axis
\* searchSameSize: \\<default: false> | If true, it will search for already existing portals that are built with the same size
\* searchFirstClonePortal: \\<default: true> | If true, it will first search for same size and same axis portals, if not, it will just search using the values above
\* enableEntitiesTeleport: \\<default: false> | If true, entities will teleport (teleport delay always applies to them)
\* updateEveryTick: \\<default: 7> | This is every how many ticks portals will check for entities nearby in order to teleport them. (This does not apply to players)

You can also set the min/max world heights in the config like that:

\`\`\`yaml
Worlds:
  <world name>:
    MinHeight: <min Y that you want portals to teleport to>
    MaxHeight: <max Y that you want portals to teleport to>
    Size: <the size of the world as if you were going to change the world border>
\`\`\`

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/dimensions-configuration.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.