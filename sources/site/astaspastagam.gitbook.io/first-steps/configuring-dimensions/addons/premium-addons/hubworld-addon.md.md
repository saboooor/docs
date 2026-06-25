# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/hubworld-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/hubworld-addon.md).

# HubWorld addon

## What does it do?

Hub world allows you to set a world as a "hub" for a specific portal. Doing so will give you the chance to set up a nice little spawn that every player can get to from any location on the map by building a portal. Using a portal to teleport to the hub and using the portal from the hub again, will teleport them to the last portal they used. &#x20;

## How is it configured?

\`\`\`yaml
Addon:
  Hub:
    World: '<input1>'
    Portals:
      List: \[\] #<input2>
        # - world,x,y,z
      Mode: <input3>
      
  
\`\`\`

\\<input1> = 'false' to disable it (or remove the line) or the world that you want to behave as a hub (usually the default world OR the portal world)

\\<input2> = If input1 is not 'false' then the portals list does not work. In this list you can put all the portal locations you want to set as portal hubs. If a portal is broken, its not removed from here. If ALL hub portals are broken, then the returning portals of players are lost. You dont have to manually input all the portal locations here, you can use the \*\*/dim addHub\*\* command instead (while looking at a portal)

\\<input3> = 'random' to select a random portal from the list every time the player must be teleported to a hub portal, or 'firstToLast' to teleport to the first portal (from the list) that is lit at the moment of the player teleporting

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/hubworld-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.