# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/velocity-setup.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/velocity-setup.md).

# Velocity setup

First, you need to put DimensionsVelocity.jar inside the plugins folder in your proxy.

Now, you need to open \*\*./plugins/dimensionsvelocity/config.toml\*\* and set the following to whatever suits your needs

\`\`\`
config-version: "1.0.0" # This is important, it must be included BUT NOT MODIFIED
fallbackServer: "<your main server where you want players to travel if the portal cannot find a destination portal>"
Portals: \[
    "<portalName>-><server>",
#   "examplePortal->serverOne",
#   "otherPortal->netherServer",
#   "<portalName>-><serverName>", #This will teleport the player to the specified server when the specified portal is used, and if the portal used is in <serverName> then the player would be teleported in the fallbackServer mentioned in the config
#   "<serverFrom>-><portalName>-><serverName>" #Now this will work like the above but if the portal used was in the <serverFrom> it will ALWAYS teleport to <serverName> no matter what
\]
\`\`\`

{% hint style="info" %}
The portal name is the file name of the portal in every server and must be the same otherwise the plugin is not going to function properly
{% endhint %}

Now you need to move to your spigot/paper server to complete the setup

{% content-ref url="/pages/6zAjDlGPQ6lsckib9ND3" %}
\[Spigot/Paper setup\](/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/spigot-paper-setup.md)
{% endcontent-ref %}

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/velocity-setup.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.