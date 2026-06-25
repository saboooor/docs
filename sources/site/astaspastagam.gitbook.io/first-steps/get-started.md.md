# Source: https://astaspastagam.gitbook.io/first-steps/get-started.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/get-started.md).

# Get Started

{% hint style="success" %}
This wiki has been updated for the Dimensions 3 update.
{% endhint %}

## Installing Dimensions

To install dimensions the only thing you need to do is as simple as dragging the \*\*Dimensions.jar\*\* you downloaded into the \*\*plugins\*\* folder inside your Minecraft server files.

After you have done that, restart your server and the plugin will be ready for use.

## Creating a portal

To create a portal, you need to go to <https://astaspasta.alwaysdata.net/> and click on the Portal creator. From there, you can fully customize your portal.

Once you have finished, go to the "Config" tab and click \*\*Download portal file\*\*. Now you need to put that .yml file you just downloaded in the \*\*./plugins/Dimensions/Portals/\*\* folder. Restart your server again, and you are ready to go.

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/get-started.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.