# Source: https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/customportal.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/dimensions-api/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/customportal.md).

# CustomPortal

## Creating a new portal

You should not create a CustomPortal since it should only be loaded by the \[CustomPortalLoader\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/customportal/CustomPortalLoader.html) from the \*\*./plugins/Dimensions/Portals/\*\* directory.

## Overriding portal

Addons should not have much control over the CustomPortal that is being loaded since they are supposed to \*add\* features to Dimensions and not override them. But there are these methods that you can use to override Dimensions portals without too much work and event cancelling:

\* \[CustomPortal#setInsideBlockData(BlockData)\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/customportal/CustomPortal.html#setInsideBlockData\\(org.bukkit.block.data.BlockData\\))
\* \[PortalGeometry#setCustomGeometry​(CustomPortal, PortalGeometry)\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/completePortal/PortalGeometry.html#setCustomGeometry\\(me.xxastaspastaxx.dimensions.customportal.CustomPortal,me.xxastaspastaxx.dimensions.completePortal.PortalGeometry\\))

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/customportal.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.