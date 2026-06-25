# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/particles-addon/particles-editor.md

\> For the complete documentation index, see \[llms.txt\](https://astaspastagam.gitbook.io/first-steps/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/particles-addon/particles-editor.md).

# Particles Editor

{% hint style="warning" %}
The portal inside the editor cannot be rotate \*\*yet\*\* and all particles will seem like they are in the same Z axis. Don't worry, they are not.
{% endhint %}

{% hint style="info" %}
The particles editor is a tool that simulates the particles spawning. It's supposed to make creating particle packs easier
{% endhint %}

!\[Example of the editor\](/files/sUuTSUNCD0IO9jqJ4qyV)

We are going to create the same example from \[here\](/first-steps/configuring-dimensions/addons/premium-addons/particles-addon.md#example), but this time using the particle editor.

First, we have the \*\*start\*\* block and we instantiate any variable we want to use, which are:

\* amount = 50
\* radius = 4
\* increment = (2 \\\* 3.14) / amount
\* frequency = 20

In order to add these variables to the start block, we have to click at \*\*start\*\* in the \*\*Explorer\*\* and the \*\*Assets\*\* window will update to show us all the available options. We click at \*\*Variable\*\* and then at the right part of your screen you click on \*\*Add\*\*.

<div align="center"><img src="/files/2rXJAGIxG3JsJZWvONaU" alt=""></div>

After you have pressed \*\*Add\*\*, \*\*tempVariable\*\* will be added to \*\*start\*\*.

<div align="center"><img src="/files/P1GB9ufmaFdWASzohrcL" alt=""></div>

Now click at \*\*tempVariable1\*\* and look at the right of your screen.

!\[\](/files/EFhQvEP690rGzUnT4VVA)

Now we change the name to \*\*amount\*\* and the value to \*\*50\*\* and we click \*\*Save\*\*.

We repeat that for all the variables we need, and we end up with:

!\[\](/files/eEU2l88D3998qcc4WktE)

Now that we have set up some of the variables we will be needing, we will now head to the main body of the "pack".&#x20;

For this example, we want to use a \*\*for\*\* loop, for the center of the portal, so we will use \*\*portal\*\* and not \*\*tile\*\*

So in order to create a circle around the portal we will need these:

\* A for loop where \*\*i\*\* starts with the value \*\*0\*\* and the for loop runs only while \*\*i\*\* is less than the \*\*amount\*\* (that we set at \*\*start\*\*). And after each run of the loop, we want to increase \*\*i\*\* by \*\*1\*\*.
\* Inside the loop we need to add a runnable so we put some code to run and inside the runnable we add
\* Inside the for loop we add these variables (to create a circle)\\
 angle = i\\\* increment\\
 x = locX + (radius \\\* cos(angle))\\
 z = locZ + (radius \\\* sin(angle))
\* And lastly we add a particle that plays \*\*REDSTONE\*\* at \*\*x locY z 3 0 0 0\*\* and has \*\*DustOptions(Color(0,255,0),2)\*\*

For the for loop we click at \*\*portal->for\*\* and then at the assets we click on \*\*For loop\*\* (it will add a runnable automatically) and we set it like that

!\[\](/files/Pp6o9pzuso6z0Dyz6Oyb)

Then we add the variables inside the runnable and we end up with this:

!\[\](/files/CYgHLaCFf4G388IOQ4FS)

Finally we add our particle which should look like this:

!\[\](/files/wbi0W6jnVtAEvwuW3SDH)

And now if we click on \*\*Run\*\* it will show us how it will look in minecraft:

!\[\](/files/IeWbpnBYchRVWTcWjptR)

---

# Agent Instructions
This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com.

## Querying This Documentation
If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question.

Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter:

\`\`\`
GET https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/particles-addon/particles-editor.md?ask=<question>&goal=<endgoal>
\`\`\`

\`ask\` is the immediate question: it should be specific, self-contained, and written in natural language.
\`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal.

The response will contain a direct answer to the question and relevant excerpts and sources from the documentation.

Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.