# Source: https://astaspastagam.gitbook.io/dimensions-api/creating-an-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/dimensions-api/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/dimensions-api/creating-an-addon.md).

# Creating an addon

{% hint style="info" %}
\[Source code\](https://github.com/xXastaspastaXx/Dimensions3) & \[Javadocs\](https://astaspasta.alwaysdata.net/javadocs)
{% endhint %}

## Main class

Your main class should extend \[DimensionsAddon\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/addons/DimensionsAddon.html)

{% hint style="info" %}
If you want to use the\[ Dimensions events\](https://astaspasta.alwaysdata.net/javadocs/me/xxastaspastaxx/dimensions/events/package-summary.html) then your class must also implement\[ Listener\](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/event/Listener.html)
{% endhint %}

## META-INF

When you are done coding, you have to let Dimensions know about the addon otherwise its not going to load it.

You need to create a few folders and files inside our \*\*src\*\* folder.

\`\`\`
src
└───main
    └───java
        └───META-INF
            └───services
\`\`\`

Inside the \*\*services\*\* folder you need to create a new file named:

\`\`\`
me.xxastaspastaxx.dimensions.addons.DimensionsAddon
\`\`\`

Finally, inside the file, enter the path to your main class as you would with \*\*plugin.yml\*\*

{% hint style="info" %}
This part is required by \[ServiceLoader\](https://docs.oracle.com/javase/8/docs/api/java/util/ServiceLoader.html) in order to load the addons properly
{% endhint %}

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/dimensions-api/creating-an-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.