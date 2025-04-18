# TermART
TermART is a Python module that simplifies the use of ANSI escape codes to style your terminal output. Add colors, effects easily with clean and readable functions. Perfect for CLI tools, TUI apps, or just making your terminal scripts look cooler!

## Function
### 1. Reset 
Reset your text colour, style to default
```python
from TermART import *

reset("Font_style")       # Reset all font style
reset("Bold")             # Reset only Bold font style
reset("Underline")        # Reset only Underline font style
reset("Italic")           # Reset only Italic font style
reset("tc")               # Reset text colour
reset("bg")               # Reset Background colour 
reset()                   # Reset every style, colour, bg colour
```
### 2. Text colours (tc & tc_rgb)
Changs your text colour :
```python
from TermART import *

#tc()
print(tc("RED") + "This is red text" + reset("tc")) #Set red colour by "RED","RED","GREEN","BLUE","YELLOW","MAGENTA","CYAN","WHITE" and "BLACK"

#tc_rgb(r,g,b)
print(tc_rgb(255,255,255) + "This is 255,255,255 colour text" + reset("tc")) #Set colour by rgb
```
### 3. Background colours (bg & bg_rgb)
Changs your text background colour :
```python
from TermART import *

#bg()
print(bg("RED") + "This is red text background" + reset("bg")) #Set red background colour by "RED","RED","GREEN","BLUE","YELLOW","MAGENTA","CYAN","WHITE" and "BLACK"

#bg_rgb(r,g,b)
print(bg_rgb(255,255,255) + "This is 255,255,255 colour text background" + reset("bg")) #Set background colour by rgb
```
### 4. Font styles (fs)
Chang your Font style:
>Options
>
>- Bold , Underline , Reversed and Italic
```python
from TermART import *

print(fs("Bold") + "Hi") # Set Bold style
# Options Bold , Underline , Reversed and Italic
```



