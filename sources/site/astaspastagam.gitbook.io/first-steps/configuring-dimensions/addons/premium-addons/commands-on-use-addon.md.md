# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/commands-on-use-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/commands-on-use-addon.md).

# Commands on use addon

## What does it do?

The addon gives you the ability to execute commands when a player uses the portal

## How is it configured?

\`\`\`yaml
Addon:
  Commands:
    - '<input1>;<input2>;<input3>'
\`\`\`

\* input1: who is going to execute the command (values= \*\*player\*\* or \*\*console\*\*)
\* input2: pre-conditions for the command to be executed. For example \`((%destinationWorld%==world6 && %entity%==astaspasta) || %portal%==samplePortal) && %zAxis%\`. \`true\` can be used if you want the command to run anyway
\* input3: the command to execute.

For example \`tell %entity% you used a zAxis portal and its name is samplePortal or your name is astaspasta and you came from world6\`

{% hint style="info" %}
If you plan to override the teleport of Dimensions (for example for a random location command) then It's recommended that you add the following to your portal config. (This addon option is provided by the CommandsOnUse addon)

\`\`\`yaml
Addon:
  DisableTeleport: true
\`\`\`

{% endhint %}

\`\`\`
Placeholders:
%portal% - Portal display name
%name% - Portal name
%entity% - Player name/Entity Type
%entityID% - Player UUID/Entity ID

%destinationWorld% - Destination world
%destinationX% - Destination X
%destinationY% - Destination Y
%destinationZ% - Destination Z

%originalWorld% - Original world
%originalX% - Original X
%originalY% - Original Y
%originalZ% - Original Z

%zAxis% - True if portal is Facing the X Axis (aka portal is build along the Z Axis

The CommandsOnUse Addon also supports PlaceholderAPI placeholders
\`\`\`

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/commands-on-use-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.