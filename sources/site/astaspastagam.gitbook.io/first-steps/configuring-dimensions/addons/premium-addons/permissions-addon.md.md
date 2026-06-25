# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/permissions-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/permissions-addon.md).

# Permissions addon

## What does it do?

You can set permissions for each portal using this addon. Players that do not have permissions will not be able to ignite or use the portal.

## How is it configured?

\`\`\`yaml
Addon:
  Permission:
    Node: '<input1>'
    DenyMessage: '<input2>'
\`\`\`

\* \\<input1> = 'none' to disable or any string text you want to be the permission (e.x dimensions.useportal.samplePortal)
\* \\<input2> = any string text you want to be shown to the player if they dont have permission

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/permissions-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.