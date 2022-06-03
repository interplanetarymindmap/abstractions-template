---
prop-name-1612697362: PIPMM instructions
prop-abstract-1612698044: Initial instructions that a PIPMM user will see after the first installation
---

If you are seeing this in the browser for first time... Congratulations! you made it very far! The installation seems to be working :)
The following is a set of instructions to guide you for how to start using PIPMM.

The get a better understanding of what is going on open the  "abstractions-template" repository that you just clonned with Visual Studio Code

Look for the following file in VS Code:

- Open the "search by name command" using `ctrl + p`
- Type in "hello-world-1644425608"

Now, save that file. Just `ctrl + s`

The browser should have been updated rendering the Hello World file.

Now you play around...

Some things that may help you start:

Hot reload

- When you run "pipmm watch" as you just did a "hot-reload" is enabled, which will allow you to preview the changes in VSCode in the browser

Friend's abstractions:

- In VSCode you will see a folder named "xavi-YAxr3c", these are my (Xavi) abstractions.
- In particular are some of the abstractions necessary for the renders that you see in the browser to work.
- You should not edit or changes those abstractions, as it will be the equivalent to changing my mind. You can't do that.

Your abstractions:

- Your abstractions go at the root folder
- If you just started there is only one "fake" abstraction named "hello-world-1644425608". This one is all yours...
- Play around with editing its content to see how it effect what's render in the browser
  
Creating new abstractions:

- open the "hello-world-1644425608" file, and somewhere in the body of the file type: "iid". A dialog mentioning "Intent ID" should appear. Press return.
- This will create a template to create the correct naming for your new abstraction. Just type the name that represents the abstraction for you (lower case and without spaces)
- If you ctrl+click the abstraction, a new note will be created with the name in the root folder.
- Your abstraction is empty though. If you click into the newly created abstraction file body and type "view", another dialog will appear. Press return.
- Now you just created a template for your new abstraction that you can populate.

Editing templates:

- The "templates" used to create the "iid" and the "view" are called "snippets", and is a VSCode feature that allows you to build your own templates.
- This template is just what I (Xavi) usually use, and its useful to start, but the goal here is for you to eventually generate and work with your own templates and properties.
- If you want to explore that further you can read the (([[trans-ipt-hyperlink-1648046072]],<https://code.visualstudio.com/docs/editor/userdefinedsnippets>, VSCode documentation about code snippets)). You will find the file at ".vscode/Reference.code-snippets"
