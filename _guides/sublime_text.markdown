---
title: Sublime Text Setup
section: guides
layout: page
---

Sublime Text
============

A guide to setting up Sublime Text to maintain the best coding standards and maximise your productivity

Use the right configuration options
---------------

* Make sure to configure the Sublime Text to use soft-tabs. You can change that settings in Preferences -> Settings (User). Example:

  ```JSON
    {
      "detect_indentation": false,
      "tab_size": 2,
      "translate_tabs_to_spaces": true
    }
  ```

* Make the editor work for you. Use whatever color scheme, font size, key-bindings etc. that suit your preferences. As long as you're conforming to the style guidelines, you're all good

Supercharge Your Environment With Package Control
---------------
Sublime Text is a good editor out of the box, but you can turn it into a great one by using Package Control!

[Package Control](https://packagecontrol.io/)

Follow the installation instructions at the link below, it's all quite straightforward

[Installation](https://packagecontrol.io/installation)

After installing the Package Control, you can install new plugin straight out of Sublime Text command pallette (```cmd+shift+p``` on Mac OS X, ```ctrl+shift+p``` on Linux/Windows).

* Just select ```Package Control: Install Package``` from the command pallette and find the plugin you want to use to install it

* Pretty much all packages are hosted on Github, make sure to always follow the installation instructions found in the package documentation to see whether any new changes/settings need to be added to your configuration files

* For instance, package like Sublime Linter needs to be able to find linter executables. It looks at the paths in your environment ```PATH``` variable, but you can add specific paths like your RVM ruby in the package config file.

* Example, in my Preferences -> Package Settings -> SublimeLinter -> Settings - User, I've added the path declaration so all my linter executables are found:

  ```JSON
    "paths": {
      "linux": [],
      "osx": [
          "/Users/Tomasz/.rvm/gems/ruby-2.3.1@global/bin/",
          "/Users/Tomasz/.rvm/gems/ruby-2.2.2@global/bin/",
          "/usr/local/bin/"
      ],
      "windows": []
  }
  ```

If the package is not working. Make sure it is designed to work with your version of Sublime. Also View -> Show Console should give you some information about missing executables, wrong declarations and such. Some packages like SublimeLinter got their own debug mode to make fixing any issues even easier.

Useful packages
-----------

Below is the list of some of my favourite packages and quick overview of some of their functionality

* [All Autocomplete](https://github.com/alienhard/SublimeAllAutocomplete)

  By default, Sublime autosuggests you code based on the open file. With this extension, it will autosuggest methods/variables/etc from other open files. Great when jumping back between couple of different files, putting controller variables in the view and such

* [Better CoffeeScript](https://github.com/aponxi/sublime-better-coffeescript)

  For those fond of CoffeeScript, syntax highlighting, completions and other niceties

* [CoffeeCompile](https://github.com/surjikal/sublime-coffee-compile)

  For those not as confident with their CoffeeScript chops, this lets you preview the compiled JavaScript to easily identify errors

* [Color Picker](https://github.com/weslly/ColorPicker)

  One for the front-end people, nice and pretty Color Picker. No more referencing those hex values from elsewhere!

* [Emmet](https://github.com/sergeche/emmet-sublime)

  Speed up your development of HTML and CSS. Want to code up a 6 elements list in one line? HTML5 boilerplate? This one's for you

* [GitGutter](https://github.com/jisaacks/GitGutter)

  Allows you to see differences you made from the current git revision. Good for tracking what's new and those pesky unwanted branch checkouts

* [Sidebar Enhancements](https://github.com/titoBouzout/SideBarEnhancements)

  Cut, copy, paste, duplicate files straight from within Sublime. Why this isn't part of the default installation is a mystery. A must have

* [SublimeLinter](SublimeLinter3)

  A game changer. No more missing end statement. No more unclosed brackets. No more syntax issues. SublimeLinter will give you a nice and verbose warnings when you try to do something that will make your code fail.

  This one is bit different because on its own, it doesn't do anything. You need to install language specific linters (as a package control plugins) to enable the functionality. I mostly use [Ruby linter](https://github.com/SublimeLinter/SublimeLinter-ruby) but there's one for nearly every programming language/framework imaginable.

  With linters, always, ALWAYS read the installation instructions to make sure you've got required executables available and loaded in your path.

* [Trailing Spaces](https://github.com/SublimeText/TrailingSpaces)

  Highlight trailing spaces and delete them in bulk. You'd be surprised how many of those are lurking in your code.


Learn the power of Sublime Text
-----------
Sublime is a great tool but takes a while to get used to it. There's also some not-so obvious functionalities that will change the way, you use the editor (I for one was blissfully unaware that I can just press ```cmd+r``` to jump to any definition in the Ruby file!)

There are some great guides out there and I'd wholeheartedly recommend reading/watching some of them to learn how you can use Sublime effectively.

My personal recommendation is [Tutsplus video tutorial](http://code.tutsplus.com/courses/perfect-workflow-in-sublime-text-2). It's a longer one (nearly 2 hours!) and made for Sublime Text 2, but everything still applies. It is freely available, you just need to register for an account on Tutsplus. After you watch this one, you'll be a true Sublime ninja

Final word
-----------
I love Sublime, but many people don't. There're many Vim, Emacs, Atom faithful out there. That's all perfectly fine.

Editor is a tool. An important one, but tool nonetheless. Don't use editor because everyone uses it. Use one that you're familiar with and suits your style/preference. Whatever you use, just make sure your config (tabs/syntax/etc) follow our [Coding standards](https://cleversteam.github.io/guides/ruby_rails_style_guide.html). Simple as that!
