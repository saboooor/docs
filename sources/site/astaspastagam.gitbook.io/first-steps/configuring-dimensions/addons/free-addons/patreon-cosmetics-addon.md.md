# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/patreon-cosmetics-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/patreon-cosmetics-addon.md).

# Patreon Cosmetics addon

## What does it do?

The addon gives cosmetic benefits to the users who have donated/subscribed to patreon

## How is it configured?

The addon does not need to be configured, its plug & play. Players that have linked their minecraft & patreon accounts in the Dimensions website, will be able to use their benefits in the server.

The server owners are not obligated to use the addon but it would support the plugin if they did and as a Thank you they get to use the benefits in their own server. They can do so by setting the following values in the config.yml

\`\`\`yaml
CosmeticsAddon:
    PlayerUUID: <your uuid>
    IgnitePortal: <cosmetic>
    DestroyPortal: <cosmetic>
    UsePortal: <cosmetic>
\`\`\`

Currently there are only 5 comsetic options. But many more are coming very soon

\* NOTHING - disables the effects
\* FINAL\\\_SPARK | use, destroy, ignite
\* FILLING\\\_THE\\\_VOID | tick, use, destroy, ignite
\* HEART\\\_SEEKER | tick, use, destroy, ignite
\* HUNGRY\\\_HOUNDS | tick, use, destroy, ignite
\* GLOWING\\\_AURA | tick
\* ANGRY\\\_LLAMA | tick
\* EXPLOSIONS | destroy, use
\* LIL\\\_RING | tick

The words after the effects have the following meaning:

\* use = you can put it at UsePortal
\* ignite = you can put it at IgnitePortal
\* destroy = you can put it at DestroyPortal
\* tick = you can put it at PortalTick

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/patreon-cosmetics-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.