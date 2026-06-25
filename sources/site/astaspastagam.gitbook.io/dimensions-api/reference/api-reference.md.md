# Source: https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/dimensions-api/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference.md).

# API Reference

Dive into the specifics of each API endpoint by checking out the documentation.

{% hint style="info" %}
You might be interested in:

\* \[DimensionsSettings\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/DimensionsSettings.html)
\* \[DimensionsUtils\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/DimensionsUtils.html)
\* \[DimensionsDebbuger\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/DimensionsDebbuger.html)
 {% endhint %}

## CustomPortal

All the methods associated with the registered custom portals:

{% content-ref url="/pages/ypJSZSlPvkHnEfMkaOaD" %}
\[CustomPortal\](/dimensions-api/reference/api-reference/customportal.md)
{% endcontent-ref %}

## CompletePortal

Everything related to portals existing in the world:

{% content-ref url="/pages/LTs2cUyN32Z2QASJGhUM" %}
\[CompletePortal\](/dimensions-api/reference/api-reference/completeportal.md)
{% endcontent-ref %}

## PortalGeometry

If you want to override Dimensions check for portal structures

{% content-ref url="/pages/Ii6dOVlrha2ifEPJ5KUP" %}
\[PortalGeometry\](/dimensions-api/reference/api-reference/portalgeometry.md)
{% endcontent-ref %}

## Events

The events that Dimensions will call and you can listen to change the behavior of portals:

{% content-ref url="/pages/BBUWerk1cLr92chR0ajM" %}
\[Events\](/dimensions-api/reference/api-reference/events.md)
{% endcontent-ref %}

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/dimensions-api/reference/api-reference.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.