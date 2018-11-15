## Mett's Dark Snek Syntax theme

A syntax highlighting theme for MagicPython based off 'One Dark' with lots of tweaks to the existing colors and several Python-specific syntax highlighting features not taken advantage of in the original.

It blends in cleanly with the 'One Dark' UI theme, but any dark ui theme should do.

Non-python languages will still retain the base syntax highlighting from the 'One Dark' syntax theme.


![dark-snek-syntax](https://github.com/Mettpawwz/dark-snek-syntax/blob/master/MettDarkSnek.PNG?raw=true)


### Install

Search for it under __Install__ in the Atom settings menu. Make sure to look for __Themes__ and not __Packages__. It can then be activated by going to the __Settings > Themes__ section and selecting it from the __Syntax Themes__ drop-down menu.

### Colors
<pre>
teal        - for built-ins, magic methods, types etc.
orange      - Class name color in class def and various misc uses (such as the curly braces in f-strings, constants, the ellipsis, etc.)
yellow      - for 'class', 'def', and 'lambda' keywords

darkblue    - for functions and method names in defs, as well as in calls
lightblue   - for singletons (None, True, False), numeric literals (1, 1.5, 2e3, etc.), and, arithmetic operators (+, -, \*, /, //, %, etc.)

lightpurple - for flow control (for, while, if, else, try, except, finally, with, raise), and imports
darkpurple  - for function and method arguments (except those highlighted especially as lightred), and all assignment operators (=, +=, etc.)

lightgreen  - for strings
darkgreen   - for logical operators (and, or, not, in, is), comparison operators (==, !=, >, <, etc.) and bitwise operators (&, |, ~, etc.). Basically anything that resolves to True or False.

lightred    - for important non-keyword variable names like 'self', 'cls', etc.
darkred     - for errors
</pre>

I've also redone the regex syntax (available for strings that are preceded by a lower-case 'r') like so:

<pre>
teal        - for normal characters that match themselves
orange      - for named group assignments (e.g. '(?P<SomeName>SomeRegex)')
yellow      - for the start-of-string ('^') and end-of-sring ('^') anchors and the match-anything operator ('.')

darkblue    - for character groups (e.g. '[abc]', '[A-Za-z0-1]')
lightblue   - for ordinary escaped sequences with no special meaning (e.g. '\\(', '\\.')

lightpurple - for special escaped characters (e.g. '\\d', '\\w')
darkpurple  - for the opening and closing parentheses of capture groups as well as backreferences to previous capture groups (e.g. '\\1', '(?P=SomeName)')

lightgreen  - for forward-references ('(?=SomeRegex)') and back-references ('?<=SomeRegex')
darkgreen   - for quantifiers (e.g. '\*', '+', '?', '{1,3}', etc.)

lightred    - for negated forward-references ('(?!SomeRegex)') and negated back-references ('?<!SomeRegex')
darkred     - for the negation operator ('^') in a character group (e.g. '[^abc]')
</pre>

Everything else is unchanged from the One Dark theme.
