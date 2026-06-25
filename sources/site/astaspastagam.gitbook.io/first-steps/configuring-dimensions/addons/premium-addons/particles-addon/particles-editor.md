# Source: https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/particles-addon/particles-editor

For the complete documentation index, see [llms.txt](https://astaspastagam.gitbook.io/first-steps/llms.txt). This page is also available as [Markdown](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/particles-addon/particles-editor.md).

The portal inside the editor cannot be rotate **yet** and all particles will seem like they are in the same Z axis. Don't worry, they are not.

The particles editor is a tool that simulates the particles spawning. It's supposed to make creating particle packs easier

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FdVV0m66lo5gqzkHBVsCy%252Fimage.png%3Falt%3Dmedia%26token%3D48c45ef7-663d-444d-b732-6ea298558682&width=768&dpr=3&quality=100&sign=1ef43ceb&sv=2)

Example of the editor

We are going to create the same example from [here](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/particles-addon#example), but this time using the particle editor.

First, we have the **start** block and we instantiate any variable we want to use, which are:

- amount = 50
 
- radius = 4
 
- increment = (2 \* 3.14) / amount
 
- frequency = 20
 

In order to add these variables to the start block, we have to click at **start** in the **Explorer** and the **Assets** window will update to show us all the available options. We click at **Variable** and then at the right part of your screen you click on **Add**.

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252F5U173HfpXLkFYJOD65rp%252Fimage.png%3Falt%3Dmedia%26token%3D4a1de396-5f93-43e0-9272-1db2885657dd&width=768&dpr=3&quality=100&sign=78dfc12d&sv=2)

After you have pressed **Add**, **tempVariable** will be added to **start**.

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FXl7ROwqW291cqn9K1pIk%252Fimage.png%3Falt%3Dmedia%26token%3D20bc1091-7f5b-4304-b680-5b91542be007&width=768&dpr=3&quality=100&sign=206a006f&sv=2)

Now click at **tempVariable1** and look at the right of your screen.

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252F3OxABtuQ1KUSVjtb4V3K%252Fimage.png%3Falt%3Dmedia%26token%3Daa5f414f-d8ea-4020-afdf-ce81068a0181&width=768&dpr=3&quality=100&sign=32c866f2&sv=2)

Now we change the name to **amount** and the value to **50** and we click **Save**.

We repeat that for all the variables we need, and we end up with:

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FdJcBJ3NqhSBBtQuvlAOt%252Fimage.png%3Falt%3Dmedia%26token%3D0542f282-d26f-4a6f-ad5c-3841ea3f3170&width=768&dpr=3&quality=100&sign=ed6e6d6f&sv=2)

Now that we have set up some of the variables we will be needing, we will now head to the main body of the "pack".

For this example, we want to use a **for** loop, for the center of the portal, so we will use **portal** and not **tile**

So in order to create a circle around the portal we will need these:

- A for loop where **i** starts with the value **0** and the for loop runs only while **i** is less than the **amount** (that we set at **start**). And after each run of the loop, we want to increase **i** by **1**.
 
- Inside the loop we need to add a runnable so we put some code to run and inside the runnable we add
 
- Inside the for loop we add these variables (to create a circle) angle = i\* increment x = locX + (radius \* cos(angle)) z = locZ + (radius \* sin(angle))
 
- And lastly we add a particle that plays **REDSTONE** at **x locY z 3 0 0 0** and has **DustOptions(Color(0,255,0),2)**
 

For the for loop we click at **portal->for** and then at the assets we click on **For loop** (it will add a runnable automatically) and we set it like that

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FK0Aftx7ErIVdGGHw4DGq%252Fimage.png%3Falt%3Dmedia%26token%3D40234fcc-920f-4683-be6b-20b09135c9ab&width=768&dpr=3&quality=100&sign=2dd3db9f&sv=2)

Then we add the variables inside the runnable and we end up with this:

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FjpcnBR46GehkQghh78iT%252Fimage.png%3Falt%3Dmedia%26token%3Df1660959-51d3-432f-923d-7e7880e16bd2&width=768&dpr=3&quality=100&sign=6ff3e1c7&sv=2)

Finally we add our particle which should look like this:

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FsyMv8dNRx3gUamXBNeOT%252Fimage.png%3Falt%3Dmedia%26token%3Dd35e84e4-f52c-4b5d-8ad8-6fa89339ce6d&width=768&dpr=3&quality=100&sign=148cc107&sv=2)

And now if we click on **Run** it will show us how it will look in minecraft:

![](https://astaspastagam.gitbook.io/first-steps/~gitbook/image?url=https%3A%2F%2F1092078244-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdhucfF0MgHVNT2etrhvq%252Fuploads%252FB82c3UN4cQdGC0QXraz3%252Fimage.png%3Falt%3Dmedia%26token%3D15bff043-6716-4d8d-ad8c-eb77f5378c1c&width=768&dpr=3&quality=100&sign=8f092f42&sv=2)

[PreviousParticles addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/particles-addon) [NextBungee addon](https://astaspastagam.gitbook.io/first-steps/configuring-dimensions/addons/premium-addons/bungee-addon)

Last updated 3 years ago