# Source: https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/events.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/dimensions-api/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/events.md).

# Events

## \[CustomPortalUseEvent\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/events/CustomPortalUseEvent.html)

The event is fired when an entity or a player uses a portal and is ready to be teleported

If the event is cancelled the player will not be teleported

## \[CustomPortalIgniteEvent\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/events/CustomPortalIgniteEvent.html)

The event is fired when a portal is being ignited

If the event is canceled the portal will not be ignited

## \[CustomPortalBreakEvent\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/events/CustomPortalBreakEvent.html)

The event is fired when a portal is being broken

If the event is canceled the portal will not break

{% hint style="warning" %}
If you use the \*\*Dimensions#getCompletePortalManager()#removePortal()\*\*

Then you may want to revert the block states or the situation that caused the event because the portal will stay lit but the frame might be missing (in case you run the command when blocks break, etc)
{% endhint %}

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference/events.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.