---
title: Top 5 VSCode Tricks
date: 2019-12-01T18:49:23.445Z
thumb_img_path: /images/top-10-vscode-tricks.webp
content_img_path: /images/top-10-vscode-tricks.webp
template: post
---
## 1) Toggle Intellisense suggestions

Intellisense is pretty good about automatically suggesting autocomplete options, but sometimes VSCode doesn't automatically show you the list of autocomplete options and you might want to toggle it on. To do this you can use the shortcut: **Control + Space**

Try it out! You'll notice that it brings up a list of suggestions that might be helpful to you in your current context. For example, if you are pulling in a specific module from a library, you can hit **Control + Space** inside of the brackets to pull up the list of modules exported from that library.

## 2) Hyperlink to module

In previous code editors, to find a file you were importing you'd have to go to your file explorer and count the amount of directories you were going back and then how many you were going forward. Things would look somewhat like this: **../../../components/Footer.js**

Now, thanks to VSCode and the work of previous code editors like Sublime and Atom we are able to **Command + Click** on a specific module to open up the file in a new tab. This has saved me countless  seconds of traversing through the file directory in order to find a specific module that I need to edit.

_Note: This will not only work for JS files, but SASS files as well!_

## 3) See what's available in an object

Using Intellisense, we're able to pull in the list of available methods or properties inside of a given object. This can be extremely useful if you forget the name for a method in a library, but don't want to go all the way into the documentation of that library to find the name.

In this scenario, your memory will get jolted and you'll even find a useful description for the method you're looking for as long as the library author was using JSDocs. Try this out by importing the underscore from the lodash utility library and see what happens when you type the period after the underscore like this: **_.**

**Use tip one if nothing comes up!**

## 4) Turn on checkJS in your config for "Typescript Lite"

The type inferencing that VSCode gives you out of the box is amazing! If you're not ready to dive deep into Typescript, you'll still be able to use some of it's benefits like the type inferencing that VSCode gives you in your javascript files when you turn on this option in your VSCode JSON Config:

```
"javascript.implicitProjectConfig.checkJs": true
```

Based on what you initialize a variable as, VSCode will be able to keep track of this variable and give you warnings when you attempt to use a method that's not supported for that type. For example, say you have a number and then try to map through that number. Now you'll get an error message stating that this method is not available for the type you're trying to invoke it on.

## 5) Import a module just by typing the export name

Instead of going all the way to the top of a file to import a module, you can also import a module just by typing the exported name of that module and pressing enter when you see it come up in the Intellisense autosuggestions. This is a great shortcut that you can use in place of importing a module at the top of the file and then calling that function later on in your code.

_I hope you've found this article useful! Please let me know if you have any questions or concerns with any of the information provided in this article._

[Don't hesitate to ask, you can reach me here!](https://geoffcodes.com/contact/)
