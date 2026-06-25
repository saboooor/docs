# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/lightapi-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/lightapi-addon.md).

# LightAPI addon

## What does it do?

Portals now emit block light

{% hint style="info" %}
Requires \[LightAPI\](https://www.spigotmc.org/resources/lightapi.4510/) 5.3.0
{% endhint %}

{% hint style="warning" %}
After the recent paper update, LightAPI requires the following settings in order to work

\`\`\`
enable-compatibility-mode: true
force-enable-legacy: true
\`\`\`

Using these settings may impact server performance
{% endhint %}

## How is it configured?

\`\`\`yaml
Addon:
    LightAPI:
        Level: <input>
\`\`\`

Level can be 0-15.\\
Recommended light level = 10

### Portal without light vs Portal with light

!\[\](/files/mHWD2IWvH8GJjY2xH8eA)!\[\](/files/7f53SU1S21UglI7LpCaV)

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/free-addons/lightapi-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.