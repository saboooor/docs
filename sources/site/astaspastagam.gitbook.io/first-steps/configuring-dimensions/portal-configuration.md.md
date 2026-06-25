# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/portal-configuration.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/portal-configuration.md).

# Portal configuration

#### Enable | default: true

Toggle the portal

#### DisplayName | default: Unnamed

The "pretty" way that the plugin talks about the portal

#### Portal.Frame.Mateiral | default: COBBLESTONE

The outside of the portal

#### Portal.Frame.Face | default: all

\\\['all','x','y','z','NORTH','EAST','WEST','SOUTH'\]

#### Portal.InsideMaterial | default: NETHER\\\_PORTAL

The block that is going to fill the inside

#### Portal.LighterMaterial | default: FLINT\\\_AN&#x44;\*\\\_\*&#x53;TEEL

The item that ignites the portal

#### Portal.ParticlesColor | default: 0;0;0

r;g;b

#### Portal.BreakEffect | default: BLOCK\\\_GLASS\\\_BREAK

\[Sounds\](https://helpch.at/docs/1.9/index.html?org/bukkit/Sound.html)

#### Options.AllowedWorlds | default: \\\[\] (empty list means that all worlds are allowed)

List all the allowed worlds. If you want to allow all worlds except a few, then list add the keyword 'all' and add the disabled worlds with '!' at the start of every world\\
Example:

\`\`\`
AllowedWorlds:
  - 'all'
  - '!world\_the\_end'
  - '!world\_nether'
\`\`\`

#### Options.BuildExitPortal | default: true

Allow exit portals

#### Options.TeleportDelay | default: 4

Delay before teleporting players

#### Options.EnableParticles | default: true

Emit particles from portals

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/portal-configuration.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.