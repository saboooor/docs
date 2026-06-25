# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/custom-lighter-addon.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/custom-lighter-addon.md).

# Custom lighter addon

## What does it do?

{% hint style="info" %}
Supports \[Oraxen\](https://www.spigotmc.org/resources/%E2%9C%85-10-%E2%98%84%EF%B8%8F-oraxen-add-items-blocks-armors-hats-food-furnitures-plants-and-gui.72448/), \[ItemsAdder \](https://www.spigotmc.org/resources/%E2%9C%A8itemsadder%E2%AD%90emotes-mobs-items-armors-hud-gui-emojis-blocks-wings-hats-liquids.73355/)& \[CustomItems\](https://www.spigotmc.org/resources/%E2%9B%8F-custom-items-%E2%9C%85-1-19-ready-%E2%9C%85-make-new-items-blocks-with-new-textures-recipes-events-actions.63848/)
{% endhint %}

The addon gives you the ability to set an item or a block with custom data to be used as a lighter, as a frame block or as an inside portal block (to replace the nether portal)

## How is it configured?

\`\`\`yaml
Addon:
  CustomLighter:
    Item: 
      - '<plugin>:<item>'
    FrameBlock: '<plugin>:<block>'
    InsideBlock: '<plugin>:<block>'
\`\`\`

Setting a custom item/block that is from minecraft its recommended to use the "\*\*/dim setLighter \\<portal>",\*\* "\*\*/dim setFrameBlock \\<portal>" ,\*\*"\*\*/dim setInsideBlock \\<portal>"\*\* commands.

If you use ItemsAdder or Oraxen plugin, you can set the custom items by using \*\*ITEMSADDER:\\<itemid>,\*\* \*\*ORAXEN:\\<itemid> or CUSTOMITEMS:\\<itemid>.\*\*

Note that after changing the custom item/blocks you need to restart the server.

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/custom-lighter-addon.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.