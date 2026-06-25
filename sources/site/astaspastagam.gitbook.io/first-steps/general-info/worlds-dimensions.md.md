# Source: https://astaspastagam.gitbook.io/first-steps/general-info/worlds-dimensions.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/general-info/worlds-dimensions.md).

# Worlds/Dimensions

Worlds or dimensions (however you want to call them) can be either imported or generated.

If you don't have a world you will need a world generation plugin such as \[Multiverse-Core\](https://www.spigotmc.org/resources/multiverse-core.390/) or \[MyWorlds\](https://www.spigotmc.org/resources/myworlds.39594/)

&#x20;Now, if you already have a world generated and you want to use that, you can put the world folder in your root server directory (where the rest of your worlds are and the spigot.jar or server.properties are) and use the name of the folder as the world in the portal config like that:

!\[\](/files/6ATAlM7bt4hVSA0j0dgT)

{% hint style="info" %}
In the \*\*./plugins/Dimensions/config.yml\*\* you can set the following:
{% endhint %}

\`\`\`yaml
Worlds:
  <world name>:
    MinHeight: <min Y that you want portals to teleport to>
    MaxHeight: <max Y that you want portals to teleport to>
    Size: <the size of the world as if you were going to change the world border>
\`\`\`

{% hint style="info" %}
The min/max option is to set the min/max Y that portals will spawn (when building exit portals)

\\
If the size is not set, then it grabs the world border's size and it's used to calculate the world ratio. (more info below)
{% endhint %}

<figure><img src="/files/DFXPUwafkbx0uPNWNH2I" alt=""><figcaption></figcaption></figure>

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/general-info/worlds-dimensions.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.