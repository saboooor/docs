# Source: https://astaspastagam.gitbook.io/first-steps/general-info/how-does-it-work.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/general-info/how-does-it-work.md).

# How does it work?

You have setup everything and you are ready to jump into your server and start having fun.

But wait! How do I use this? Do I need to use any commands or are there any limitations that might not let me use it yet?

The answer is \*\*maybe\*\*. The only limitations that the plugin has are, the ones you set in the config or by your server and stuff that are not yet possible or have not been added yet.

{% hint style="info" %}
Do not get scared. That does not mean you cant use Dimensions or that you have to do more stuff. It just means that if you want way more advanced stuff than simply have portals to teleport around, you have to spend \*\*at most\*\* 5 more minutes looking through the wiki.
{% endhint %}

The way Dimensions works in-game is very simple. So simple, some would say that the process looks kinda familiar.

You join your world, you gather the resources needed. You build a portal shaped like a nether portal (using the materials you have used in the config), you right-click the portal to ignite it using the item you have chosen in the config and \*\*BOOM!\*\* Now you and your friends can travel between worlds.

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/general-info/how-does-it-work.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.