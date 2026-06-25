# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/daylightsensor-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/daylightsensor-addon.md).

# DayLightSensor addon

## What does it do?

This addons gives you the ability to make portals only be activatable during a specific time of day (in game).

## How is it configured?

\`\`\`yaml
Addon:
  DayLightSensor:
    StartAllow: '<input1>'
    StopAllow: '<input2>'
    DenyMessage: '<input3>'
\`\`\`

\* \\<input1> = any integer
\* \\<input2> = any integer
\* \\<input3> = any string text you want to be shown to the player if the time is not in range

{% hint style="info" %}
You can set \*\*StartAllow\*\* to the time you want the portals to start being able to be ignited and you can set \*\*StopAllow\*\* to the time you want the portals to stop being able to be ignited.\\
If you set \*\*StartAllow\*\* to a higher integer than \*\*StopAllow\*\* then the portals will be able to be ignited after X & then before Y the next day.
{% endhint %}

{% hint style="info" %}
NOTE: setting the same time to min and max disables the addon
{% endhint %}

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/daylightsensor-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.