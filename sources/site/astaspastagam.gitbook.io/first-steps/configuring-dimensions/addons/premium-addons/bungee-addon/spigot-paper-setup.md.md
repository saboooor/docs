# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/spigot-paper-setup.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/spigot-paper-setup.md).

# Spigot/Paper setup

Now we are done with the the proxy, we move to our servers

{% hint style="info" %}
You have to do this for your every server that you want dimensions to teleport between servers so you can make one and copy paste to the rest.
{% endhint %}

{% hint style="warning" %}
Dimensions & BungeeAddon MUST be installed in order for the plugin to work.
{% endhint %}

For every portal you create, you need to enable the bungee feature from the config like its shown below

\`\`\`
  Bungee:
    Enable: true
    DestWorld: 'world' #DestWorld is the default world that the plugin will travel to (unless it has been linked to another portal in another world)
\`\`\`

And you are done. Now when you use portals they will send you to the server that you set in the Dimesions Proxy config and the plugin will send the players to the world that you specified in each portal config.

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon/spigot-paper-setup.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.