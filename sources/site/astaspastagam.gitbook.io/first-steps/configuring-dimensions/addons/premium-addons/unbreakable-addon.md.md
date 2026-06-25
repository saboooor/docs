# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/unbreakable-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/unbreakable-addon.md).

# Unbreakable addon

## What does it do?

With Unbreakable addon, you can make a portal indestructible from specific sources such as creeper explosions, or make the portal only breakable by destroying its blocks (and not the inside part of it)

## How is it configured?

\`\`\`yaml
Addon:
  Unbreakable:
    - '<input>'
\`\`\`

\\<input>:

\* PLAYER\\\_INSIDE # player attacks the portal inside (portal entity)
\* PLAYER #the destroyer was a player (by breaking the blocks)
\* ENTITY #the destroyer was an entity (creeper by explosion etc)
\* DISPENSER #a dispenser destroyed the portal (currently dispensers do not break the portal)
\* PISTON #a piston destroyed the portal
\* BLOCK\\\_PHYSICS #a block changed due to block behavior (dirt becomes grass etc)

{% hint style="info" %}
This option is a list. You can add more options by adding a new line and then another \*\*- \\<input>\*\*
{% endhint %}

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/unbreakable-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.