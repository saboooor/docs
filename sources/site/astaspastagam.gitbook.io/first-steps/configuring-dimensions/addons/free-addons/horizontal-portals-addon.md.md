# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/horizontal-portals-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/horizontal-portals-addon.md).

# Horizontal portals addon

## What does it do?

It gives you the option to make horizontal portals

{% hint style="danger" %}
Horizontal portals do not work custom blocks as frame. (custom portal inside and lighter works fine)
{% endhint %}

## How is it configured?

\`\`\`yaml
Addon:
  HorizontalPortal: '<input>'
\`\`\`

You can use "false", "true" and "both"

\* false: no horizontal portal
\* true: the portal is now horizontal
\* both: this portal can be built as vertical and as horizontal and they can link with each other

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/horizontal-portals-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.