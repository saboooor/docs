# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/biomes-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/biomes-addon.md).

# Biomes addon

## What does it do?

With biomes addon, you can restrict portals from being used in certain biomes.

## How is it configured?

\`\`\`yaml
Addon:
  Biomes:
    Allowed: '<input1>'
    DenyMessage: '<input2>'
\`\`\`

\* \\<input1> = 'all' to disable or list all the allowed biomes you want to allow (seperated with comma (,)) or use 'all, (list all the biomes you want to disabled seperated with comma (,) and each biome starting with (!))'. For example (all, !plains) to allow all biomes apart form plains or another example (plains) to enable only plains
\* \\<input2> = any string text you want to be shown to the player if the weather is not suitable

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/biomes-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.