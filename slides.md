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

## Unleashing Python's Full Potential in the Browser

Clemens Bachmann

---

# Who am I

<img src="./images/clemi.jpeg" width="100"/>

- Software Developer
  - Departement of algorithms and **didactics**
- Computer Science Teacher
- clemens.bachmann@inf.ethz.ch


---

# TigerJython 2012 (A bit of History)

|               |  |  |
|--------|------|-----|
|<img src="./images/jython.png" width="100"/>|<img src="./images/jython_turtle.png"  width="100"/> | <img src="./images/maqueen.webp" width="100"/>|
|Jython (Python in the JVM)| Educational Java Libraries <br> e.g. Turtle, GameGrid | Robotics

- Works on any Plattform (Windows, Mac, Linux)
- Easy installation
- Interactive Debugger
- Extended Syntax e.g.
  - repeat loop
  - autocasting of inputs

---

# TigerJython in 2020

- Python 2.7
- Does not work on any Platform (iPad / Android)
- No support for popular Python libraries written in C (numpy, scipy, matplotlib, pandas)

---

# WebTigerPython - TigerJython for the Web

- Works really on all Plattforms (Windows, Mac, Linux, Android, iPad)
- No installation needed
- WebAPIs pathe the way for Robotics
  - WebUSB
  - WebBluetooth
- WebAssembly makes it possible to run python in the Browser (Pyodide)
- Critical Requirements
  - Robotics
  - Visual Computing
  - Debugger
---

# Robotics

- WebUSB (micro:bit, calliope_mini)
- Simulation 🛠️
- IoT (oxocard) 🛠️

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAhjQGMGAjNMptGbPVq8AVEwA6EOoxacu9Xv0HCmIyZOnMYc-pwV8BQ0ZIDEm2fLIB9bABsArgGcDy4xEmO4ZAMrY4cYgAKAGYABgBKSVo4P3JESSZEpgA3ACUmAF4-WlS0AHMACzJMaKhiK2J8nihbQMiIJJSAGUzsprhqYtLyyrzq2vCkhKS0ambMrNCmKAhiFPSMyfiGxqTqIQB3KFogwYkVxLhbUfHFpgBGadn5iaZQ5dWk2nyiusfhw-Ox5JazqZm5mlbucHo8mLYOmQ3vtGsQjlBcIFzqEImAAL4AXSAA&device=micro%3Abit
---

# Robotics - WebUSB

- Single Devices have to be added for WebUSB
  - Auto-connect on plug if registered
- On Linux this has to be "activated"
- Only in Chrome
- Safari / Firefox declined to implement the feature
  - Many schools work with iPads
  - no real chrome

---
layout: iframe-2-cols
url: https://test.webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAhjQGMGAjNMptGbPVq8AVEwA6EOoxacu9Xv0HCmIyZOnMYc-pwV8BQ0ZIDEm2fLIB9bABsArgGcDy4xEmO4ZAMrY4cYgAKAEYABlCASklaOD9yREkmJKYANwAlJgBePlo0tABzAAsyTBioYitiAp4oW0CoiGTUgBksnOa4ahKyiqr8mrqI5MTktGoWrOzQpigIYlSMzKmExqbk6iEAdyhaIKGJVaS4WzGJpaZgmbmFyaZQlbXk2gLi-seRo5PxlNbz6dn5ulbsEHo8mLZOmQ3gcmsRjlBcCFwhEwABfAC6QA&device=micro%3Abit
---

# Robotics - Simulation 🛠️

- Works on any device
- No robot needed
- Not real robotics

---
layout: iframe-2-cols
url: https://test.webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAnoA96BjKW4ptGbPVpkmAKiYAdCP0HCmqMtgA29MkrQAjHLmWqmUAM5NlZKVIBuUJQFc4RgLxNgAXSkQmjgMwAGMxGpCfHzutFAQAOZwABQQAJSIUkxJTJZKHkyRZACCMBpocBBkADLWrFGxicmptgaYUNjYBcRRqRXuyWT8cAD6ghhkDkzqBmRRoRHRaADUAIyxbcnGSmSY1Gjh1rTRa-EGaABecPZRM94ETACs85VJJjgqo53wvfT9BufVdueotADWcLR7AByehA87qCB2Mi4JRHIEAWjBTA49BUgKBGiBC2Sd06amiQIAIuQoFibksVqwlFANHAlFEgQBZOCGTZweCFAxk9q3ZaYGE0ukMgBCtHWAAsyJCDEYoiUObFuYs7uExc0ACq0WzY3krAzi-gAd3KUjAAF9nEA&device=Oxocard
---

# Robotics - IoT 🛠️

- Connection over IoT
- Works on iPad
- Messages are exchanged
  - Does not work without WebTigerPython
  - Not real robotics
  - Oxocard has no wheels
---

# Robotics Summary

- WebUSB (Chrome only)
- WebBluetooth (Chrome only)
  - We don't support this right now
- No real Chrome on iPads 
  - Chrome on iPad is WebKit (Safari Engine) based
- IoT 
  - Code runs in Browser 🛠️
- Simulation works on anything 🛠️

---

# Visual Computing

- Turtle
  - The opposite of a blackbox
  - Intuitive commands (forward, left etc.)
  - Beginner friendly
- Game Frameworks
  - Advanced
  - Popular

---
layout: two-cols-header
---

# WebTigerPython Architecture

::left::

- Python (Pyodide runs in a Webworker)
  - UI does not freeze (single Threaded)
- Graphic Rendering can be done with callbacks

::right::

```mermaid
graph TD
    A[Main Thread] <-->|Interacts with| B[DOM]
    A <-->|postMessage API| C[Web Worker]
```

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAjIFdayAbOJtGbehyYAqADoRxAY3qdBAClFgARp1ZxFASnHiAxEwCSEJgBU0Aczi0ACrjIALehAK8I2VmSYA3KKrgBnJihaHih3ekkoPzI4YnEjAF4XNzIFMABxNCUmYjQeAEEIAC8oO04mAFFJAGs4IygIRE1tCD0AOXoPYJ8mG3tHcWDsOHImBqZxJkmmakEAdyDiOQBWAAYVpgB6Ua0jKdpzOxSAZgA2da2IDTAAXwBdIA
---

# Turtle / Input Function

- Webworker is Paused
- Interruptbuffer
- SharedBufferArray
- Whole Thread is halted
- Callback functions, cannot access DOM

---
layout: two-cols-header
---

# WebTigerPython Architecture 2

::left::

- Render Graphics off screen in Web Worker
  - offscreenCanvas
  - Introduced for better interactivity

::right::

```mermaid
graph TD
    A[Main Thread] <-->|Interacts with| B[DOM]
    A <-->|postMessage API| C[Web Worker]
    B -->|Contains| D[OffscreenCanvas]
    C -->|Accesses| D
```

---
layout: two-cols-header
---

# Asynchronity Problem

::left::

- Render Updates are done in the Webloop
- It is not possible to synchronously give control to webloop
- asyncio.sleep
  - only in asynchronous contexts
  - async Programming is not easy

::right::

````md magic-move
```py
from pygame import *

def render():
     #...
    display.flip()
def updateActors():
    #...
    render()
def main():
    while True:
        ...
        updateActors()
main()
```
```py
from pygame import *
import asyncio

async def render():
     #...
    display.flip()
    asyncio.sleep(0)
async def updateActors():
    #...
    render()
async def main():
    while True:
        ...
        await updateActors()
await main()
```
````

--> Even harder with class methods

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMNGbAewCcyACPAc1jgB0IeBiZgEkIaMmigAbNAC84zAAq4O8Hu06YMogBQBKHv2YBlOCwCu2ZmQAWc4mgDO2CVFw97AYwZw4EZgF5WJXU7R2dcTHsTAH0YOmI4LR5mZOYtAGYABgyCZkyMvQgCgXkwuAZWBjpsMrE4ex4vdxYAtXhMACU4Jq1s5l6AVgH8_QgBAFl0Xwk6Kp4Adys0CTkAFQZTOEQklPG6ADc5Jxcy7eSAazhce39A5ThMC_C2aOwve0jiXVPmNAAzZke9mArXuAGkogAZACiADEVgBdRDMb4pZiNMiYAAezAAtAF-t8_gDLkCQZhwe1BABxAASCKRKJS6KxzAA1PjCf9AcCgm1wQBVeSI5G-VFMroY3C4jmi5JE7lk8EAEQA8gB1ABywsZyWZUvZzAJsuYAiVDCgc2YcAODFw1gwbG-Hi8PkwvyWEi0PRyvXyBVRZOI5rmmHRiWNqOd3ggOS0ACZ-v0fT6dDl0f6UoGHEdwr8pNgvsayWI2gBhabuM66TBiStaABs-TAAF94UA
---

# Asyncify Problem Solution

- We Asyncify code for Students
- Fix Line numbers in Errors
- JavaScript Promise Integrations (JSPI) 
  - Experimental Chrome only feature
```py
import async
from pyodide.ffi import run_sync

def sync_update(url):
  resp = run_sync(asyncio.sleep(0))
```

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAjIFdayAbOJtGbehyYAqADoRx1NJ04Bjep0EAKUSigBzOBAqqAlOOxb5i2irWbtUPeIBGcdRgD6UmUv0RacQ-SYBWROJMQUzUxEoAjABsAAzuwUwcEQAsSe5axM7SnG5gAL4AukA
---

# Debugger

- Toggled in Settings
- Turtle Step by Step
- Breakpoints can be toggled during execution

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAHQmLgDMACBtAIwAoIBKRWpgUzTMITADwBeJgAY-owQoBOcMgFdFo6U36C4AG2FNREqQEY5CpSvWjT2-QP0BnOBcsDlajS3ZcmAWiZTbiYAah9OUUCAJhDaWmMmABZaZSdVPTImKVZI7lpsRQwyDjSMsm4wAF8AXS
---

# Debugger Recursion

- Every scope is displayed

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAYwBsoBnBgAgAU4AnBgewkQB0IzZsTgAzZgH1JGNGWkAKBnFpiCzaPHVQA5nACUAocObLVmTXGYBeDbDiCTplWMy6rt94MHYAjDbZOHggFfjAAKW4ACwgw9QBmADZ9bwhsDgwyBT8LexS0jIgsnPd9ZjAAXwBdIA
---

# Debugger Classes

---
layout: two-cols-header
---

# Debugger Overview

::left::
Dictionaries
<img src="./images/debugger_dict.png" alt="drawing" width="350"/>
Self Referencing Lists
<img src="./images/debugger_self_ref.png" alt="drawing" width="350"/>

::right::
Nested Lists
<img src="./images/debugger_nested_lists.png" alt="drawing" width="350"/>

---

# Conclusion

- Many things are still browser dependent.
- Except for iPads, all Features to Work
- There is some hope

# Outlook

- Educational Database library
- Bluetooth Robotics
- Multifile