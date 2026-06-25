# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/limited-uses-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/limited-uses-addon.md).

# Limited uses addon

## What does it do?

The portal can be set to auto-destruct after being used too many times.

## How is it configured?

\`\`\`yaml
Addon:
  LimitedUses:
    MaxUses: <input1>
    Action: '<input2>'
\`\`\`

\* input1: any integer above zero (0) that indicates how many times this portal can be used by any player in order to be destroyed
\* input2: you can use between 'Close' or 'Destroy'. \*\*Close\*\* will just break the portal like you would if you attacked the inside of it and \*\*Destroy\*\* will also remove the frame blocks. You can also add {explode%\\<integer 0-100>} if you want the portal to explode. The integer after the \*\*%\*\* are the chances of the portal exploding.

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/limited-uses-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.