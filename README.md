## Mett's Dark Snek Syntax theme

A syntax highlighting theme for MagicPython based off 'One Dark' with lots of tweaks to the existing colors and several Python-specific syntax highlighting features not taken advantage of in the original.

It blends in cleanly with the 'One Dark' UI theme, but any dark ui theme should do.

Non-python languages will still retain the base syntax highlighting from the 'One Dark' syntax theme.


![dark-snek-syntax](https://github.com/Mettpawwz/dark-snek-syntax/blob/master/MettDarkSnek.PNG?raw=true)


### Install

Search for it under __Install__ in the Atom settings menu. Make sure to look for __Themes__ and not __Packages__. It can then be activated by going to the __Settings > Themes__ section and selecting it from the __Syntax Themes__ drop-down menu.

### Colors

teal        - for built-ins, magic methods, etc.
orange      - Class name color in class def and various misc uses (such as the curly braces in f-strings, constants, etc.)
yellow      - for 'class', 'def', and 'lambda' keywords

darkblue    - for functions and method names in defs, as well as in calls
lightblue   - for singletons (None, True, False), numeric literals, and arithmetic operators

lightpurple - for flow control (and imports)
darkpurple  - for function and method arguments (except those highlighted especially as lightred), and all assignment operators

lightgreen  - for strings
darkgreen   - for logical operators and comparison operators

lightred    - nice red for important non-keyword variable names like 'self', 'cls', 'file', '__name__', etc.
darkred     - jarring red for Errors

Everything else is unchanged from the One Dark theme.
