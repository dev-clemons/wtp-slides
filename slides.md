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
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS (experimental)
css: unocss
wakeLock: "build"
---

# WebTigerPython what's new?

Clemens Bachmannn

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

---

# New Features
 
During the last year we have been busy and added a lot of new features!

Deployed Features

- 🐛 **Debugger** - Memory Visualisation
- 📜 **Documentation** - Searchable, Integrated, Interactive
- 🤖 **Robotics Update** - Minification, Calibration
- 🤹 **Pygame** - Ground Work for GameGrid

Features that will Deployed in the close future

- 💻 **Robotics Simulation** - built-in recording and camera view
- 🎵 **Jython Music** - export into PDF, PNGs, or even a hostable SPA
- 🗃️ **Databases** - anything possible on a webpage

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?layout=%5B%22Editor%22%2C%22Canvas%22%5D&lang=en&code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAgHMyBXWsgGzibRjZ6XJgCoAOhEmoA1nAAqnHnAAUASkkBnOGQBiabtwDC9bsJXiUUFnAgVLGiNrIAFWybO0LVm3agOtCi4XcgALdUlaOGw4ciYAVkRJJhSmamIVAEYANgAGR1SmLiyAFhLHagNuELJwtTAAXwBdIA
---

# Debugger

- Toggled in Settings
- Turtle Step by Step
- Breakpoints can be toggled during execution

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/??code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAYwBsoBnBgAgAU4AnBgewkQB0IzZsTgAzZgH1JGNGWkAKBnFpiCzaPHVQA5nACUAocObLVmTXGYBeDbDiCTplWMy6rt94MHYAjDbZOHggFfjAAKW4ACwgw9QBmADZ9bwg_Nz0A-IB2MABfAF0gA&lang=de&error_messages=&dark_mode=false&layout=%5B%22Editor%22%2C%22Console%22%5D&cascade_input=false&tutorial_size=0&debug_mode=true&vanilla_python=false&breakpoints=2
---

# Debugger Recursion

- Every scope is displayed

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAYwBsoBnBgAgAU4AnBgewkQB0IzZsTgAzZgH1JGNGWkAKBnFpiCzaPHVQA5nACUAocObLVmTXGYBeDbDiCTplWMy6rt94MHYAjDbZOHggFfjAAKW4ACwgw9QBmADZ9bwhsDgwyBT8LexS0jIgsnPd9ZjAAXwBdIA&lang=de&error_messages=&dark_mode=false&layout=%5B%22Editor%22%2C%22Console%22%5D&full_screen=false&cascade_input=false&tutorial_size=0&debug_mode=true&vanilla_python=false
---

# Debugger Classes

---
layout: iframe-2-cols
url: https://test.webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAgHMyBXWsgGzibRjZ6XJgCoAOhEmTqwgO5RaxABQBGAAzqAlGAC-AXSA&layout=%5B%22Editor%22%5D&full_screen=false&cascade_input=false&tutorial_size=0&debug_mode=true&vanilla_python=false
---

# Documentation (test)

- Searchable
- Tooltips
- Jump to Docs
- Interactive