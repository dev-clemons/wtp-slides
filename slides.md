---
# try also 'default' to start simple
theme: dracula
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS (experimental)
wakeLock: "build"
# aspect ratio for the slides
aspectRatio: 16/9
css: unocss
---

# WebTigerPython

## Placeholder

Author

---
layout: two-cols-header
---

# Who am I

::left::
- Name: Mona Lisa
- Occupation: Developer
- Email: mona@lisa.io

::right::
<div>
  <img src="./images/monalisa.jpg" width=150 class="absolute right-50px top-90px"/>
</div>

---
layout: wtp-2-cols
code: |
  from turtle import *

  forward(100)
---

# Turtle Graphics 🐢

<v-clicks>

- Basic instructions

</v-clicks>

---
layout: wtp-2-cols
code: |
  from microbit import *

  while True:
    display.show(Image.HEART)
    sleep(500)
    display.clear()
    sleep(500)
device: micro:bit
---

# BBC Micro:bit 🖥️

<v-clicks>

- Compact educational microcontroller
- Python programmable
- Built-in sensors
  - Accelerometer
  - Temperature
  - Compass

</v-clicks>

---
layout: wtp-2-cols
code: |
  import sqlite3

  # Connect to database
  conn = sqlite3.connect('example.db')
  cursor = conn.cursor()
---

# SQLite3 in Python 💾

<v-clicks>

- Embedded relational database
- No separate server process
- Lightweight and portable
- Built into Python standard library

</v-clicks>

---
layout: wtp-2-cols
code: |
  rows = 10
  print("Pyramid Pattern:")
  for i in range(rows):
      print(" " * (rows - i - 1) + "*" * (2 * i + 1))
  print()
wtpLayout: '["Editor", "Console"]'
---

# No Canvas View 💾

<v-clicks>

- Layout can also be specified
- Components
  - Editor
  - Canvas
  - Console
- Only 1 Canvas
- Specified in nested list
  - e.g. '["Editor", "Console"]'

</v-clicks>

--- 

Feel free to let me know if you need any further adjustments!