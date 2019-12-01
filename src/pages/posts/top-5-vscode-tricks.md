---
title: Top 5 VSCode Tricks
date: 2019-12-01T18:49:23.445Z
thumb_img_path: /images/top-10-vscode-tricks.webp
content_img_path: /images/top-10-vscode-tricks.webp
template: post
---
## 1) Toggle intellisense suggestions

Intellisense is pretty good about suggesting autocomplete options, but sometimes you want to toggle it so that it pulls up the current autosuggest options. To do this you can use the shortcut keys: **Control + Space**

Try it out! You'll notice that it loads brings up a list of suggestions that might be useful for you in the current moment. For example, if you are pulling in a specific module from a library, you can hit **Control + Space** inside of the brackets to pull up the list of modules exported from the libary.

## 2) Hyperlink to module

In previous code editors, in order to find a file you were importing you'd have to go to your file explorer and count the amount of directories you were going back and then however many you were going forward. It would look something like this: **../../../components/Footer.js**

Now, thanks to VSCode and the work of previous code editors like Sublime and Atom we are able to **Command + Click** on a specific module to open up the file in a new tab. This has saved me countless needless seconds of traversing through the file directory in order to find a specific module that I need to edit. Note: This will not only work for JS files, but SASS files as well!

## 3) See what's available in an object

Using intellisense, we're able to pull in the list of available methods or properties inside of a given object. This can be extremely useful if you forget the name for a method in a library, but don't want to go all the way into the documentation of that library to find the name.

In this scenario, your memory will be rejiggered and you'll even find a useful description for the method and how to implement it as long as the library author was using JSDoc commenting. Try it out by importing the underscore from the lodash utility library and seeing what happens when you type the period after the underscore like this: **_.**

## 4) Turn on checkJS in your config for Typescript Lite

The type inferencing that VSCode gives you out of the box is amazing! If you're not ready to dive deep into Typescript, you'll still be able to use some of it's benefits like the type inferencing that VSCode gives you right in your javascript files by turning on this option in your VSCode JSON Config:

```
"javascript.implicitProjectConfig.checkJs": true
```

Based on what you initialize a variable as, VSCode will be able to keep track of this variable and give you warning when you use a method that's not supported for that type. For example, say you have a number and try to map through that number. You'll get an error message stating that this method is not available for the type you're trying to invoke it on.

## 5) Import a module just by typing the export name

Instead of going all the way to the top of a file to import a module, you can also import a module just by typing the exported name of that module and pressing enter once you see it come up in Intellisense. This is a great shortcut to going through the ceremony of placing an import at the top of the file and then calling that function later on in your code.

_I hope you've found this article useful! Please let me know if you have any questions or concerns with any of the information provided in this article._

[Don't hesitate to ask, you can reach me here!](https://geoffcodes.com/contact/)
