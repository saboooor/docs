# Source: https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/completeportal.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/dimensions-api/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/completeportal.md).

# CompletePortal

## Creating a new portal

When creating a new portal, you want to use:

\`\`\`
Dimensions#getCompletePortalManager()#createNew()
\`\`\`

{% hint style="info" %}
If the portal is ready to be used. Otherwise, Dimensions will not count the portal and not teleport players.

Unless (for example) you want to create a temporary portal that will only exist as a placeholder for a forced teleport location.
{% endhint %}

## Portal tags

Portal tags are used to store data in the portal

\* \[CompletePortal#setTag\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/completePortal/CompletePortal.html#setTag\\(java.lang.String,java.lang.Object\\))
\* \[CompletePortal#getTag\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/completePortal/CompletePortal.html#getTag\\(java.lang.String\\))

{% hint style="info" %}
For example the HubWorld addon stores the return location of players as a tag
{% endhint %}

## Is Active

When you run a task for a portal but it's not necessary to run while the portal is not active (the chunk is not loaded), then you should use \[CompletePortal#isActive\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/completePortal/CompletePortal.html#isActive\\(\\))

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/completeportal.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.