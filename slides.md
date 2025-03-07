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

In Progress Projects

- 💻 **Robotics Simulation** - built-in recording and camera view
- 🎵 **Jython Music** - export into PDF, PNGs, or even a hostable SPA
- 🗃️ **Databases** - anything possible on a webpage

---
layout: center
---

# Deployed Features

---

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
layout: iframe-2-cols
url: https://test.webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAgHMyBXWsgGzibRjZ6XJgCoAOhEmTqwgO5RaxABQBGAAzqAlGAC-AXSA&layout=%5B%22Editor%22%5D&full_screen=false&cascade_input=false&tutorial_size=0&debug_mode=true&vanilla_python=false
---

# Documentation (test)

- Searchable
- Tooltips
- Jump to Docs
- Interactive

---

# Robotics Update - Minification

````md magic-move
```py
# mbalarm.py

import music

_m = ['c6:1', 'r', 'c6,1', 'r', 'r', 'r']

def setAlarm(on):
    if on:
        music.play(_m, wait = False, loop = True)    
    else:
        music.stop()
        
        
def beep():
    music.pitch(2000, 200, wait = False)
```
```py
import music
_g1=['c6:1','r','c6,1','r','r','r']
def setAlarm(on):
	if on:music.play(_g1,wait=False,loop=True)
	else:music.stop()
def beep():music.pitch(2000,200,wait=False)
```
````
<v-clicks>

| Name              | Orig (B) | Min (B) |
|-------------------|------|-----|
| callibot.py       | 3862 | 2032|
| huskylens.py      |20681 | 8244|
| mbalarm.py        | 255  | 173 |
| mbrobot_plusV2.py |14353 | 3926|
| mbrobot.py        |12056 | 3527|

</v-clicks>

---

# Robotics Update - New Robots

|               |  |  |
|-------------------|------|-----|
|Bit:bot <img src="./images/bitbot.png" alt="drawing" width="150"/>| Thetabot <img src="./images/thetabot.png" alt="drawing" width="150"/> | xgo <img src="./images/xgo.png" alt="drawing" width="150"/>|
|Minibit <img src="./images/minibit.png" alt="drawing" width="150"/>|Marsrover <img src="./images/marsrover.png" alt="drawing" width="150"/>| MotionKit 2.0 <img src="./images/motionkit.png" alt="drawing" width="150"/>|

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAYgEIB6AVwGcAnegIw3rggDcABHjIALAPYQAOlLCTZYIbgDmsOJjgAPWNgA2cZpig60vZtOkBlcQHdmAqAJgY0AlfAHWRcVnAG4xjAIiUHy-ZGICxHAAZrzE9ioYzGT2xqaY5hAA6sEpxGL6AmgpzDZ-AfYcASl4bnAA_JkAVEJKmMzYrMVwBAKivsRo0bE-EADGvhxwZNZwvAIWnd32EPEA4qwB2BkQLYOsZLgCPmMUEEp6AmLYZGhOAF7kaBIC0WKsQpsTzMwYSq_vAQdObEHYtGAsNBjDzFEStTBODTeBGQsa9DBjHSMQbnV5QKLVaQtZgBVYCGKxU52ayw-EWUnEInk0IQGpffS_c69ADWcFwVSgrHiwVWxi5AgAigBVACSABUglBRX8wfZHOgIAIdGJrq9WKotXduvEaaI1XUBJixGNuXqxDB4bd4JgAMLam1M6KMHQ6ZhjHzzZimsYiFWZaQuiRkTa-6QAWgTiYTzQEABkYiklfEukoRJnWJtbH0IjAxKFVYsoBMBBxBcWgeIxGRPQJeUdwsWlBdJtNZvMvT6_QGsOH5HJMndsO8UmIzBBJ9Pjln7dJopsHYdsH8ijApwc02hkplqDu9yla79obUDaXiN79NIF_vr-4oHZsEpj0C5kVoh5fGMSpamI-KOO8YQikCZykEKAgAEIALIAAqPn-EBNvCdxQEoag4WQAD6mhkHEcDEAAFAAlIg0gCLRS6Hr4Fi4MkcAwAAohoxRkXI9IFrgvRESR8RYThYF3pcPgAI6MGgPiMmAFHhhAJ4WmMEjJEqZBzghACCAAa-EWAAEgA8nKFgCAAvAIABMtEnqWyRCDoUC4N4NbenoWlXBAQ5zFIEA6amMpsQAcvhJkACKRRZ1k2XZAgniGSrfGqEBwNYqQmJqUDYNgcCCnOcEmQhcERdFsUCAAbAADPZloiqlDjpZlVQwBwMI-pEmzYNIQUheFABKbGpiZOmRVZAgAIwJSea6qHYUwzP5AgtVlpiWC6w1hcNLoKtZH6YINcCnGRNW9Od1UACyXVdAAcNWKRAFguiZw2TTVmSoBg-H7JNs44OQIjtLoXEA9gQOGBwHRA2R-H4dEaB6PDFEUcANUALpKVEf7avi-EiXAZGI3oVE0XR47yHjxB2EBhO9J0cAQz4djFACHy6K5lPjpqdEk741ng5DABWYgYGR30QL9sm9HIpAUHIvT809dF9KwuDUbzqu0cwjCsNEVYC5hqA4Zg1PE0jcAq3RmgTDc8LeJsrCa9rdH6gxCzMcR7GcWQxMAOSRt68ToSk1M7thvhyCA_MAL5yAIICHXhhEFu8lGx_71u0T4ZB65quv64bmBqfw3h-09mQ48B-MkowqwW6TLsU2OYBTIBLC-C-AFAVMlr2luegmrC1SOGgSKsBkrfk7RQyrRhh2It4zeu7n-cCKFEhwDPryW_9BgQ6ImCi-LkvS6wsskOQUCK7vpM79GGs76rddkgdbRL5P9L1-RyvP270x16v0ZFrckGg7Y1DaI7d4K9tZLFZMTOQWRBTznFPXKAHBLgdmpr0GOlt44KR3mvVgmpN7pSUieNiVY4Sbl8GIP8FoxAcGFidFIeFaaamcJmMkQFGDYHlr4L04xbgSB2CeOUXgBB8IEa8eupxnicLsIBH0pEfLVnyh8ea8BehZiKCkQ8HgvCagKiGK4zDWENgCDoEBSURSiWKEovWowaizmKAolY8QNLETEdIcRkikIuTch8JhLDTj2FOIwIwOgjjsLVHIUsoQE5CPkS8JIxFQL0Kkfw8gPRfFAgxL4NmBiIY_FUURfURQIBvFYKgEROUqiMBSP0VsfIBRCh2JkTEb47ABNct4Mih0OhdG8YsYZVtYHczAMdRmzBeC3FxM0zmQT7C0zAi8DgjAuztlwPlS0gop7cwCi_fKqjrJTU-qAhp4wjY2SujvJQ9d8L0OiLMlI1k4xTSmjvQmzBEAHmSMAQ6Fg9YGwmBjSawAsZHLotXeGXD4ZkVmToaIvQmhKE2Hw5gZNQGq0GUsEZ-K1BwvnARfCiK4DItReirYWL_46wpdETAhNJpIsZT89GULXb0uRZgE4bzvw8sJpgFOfKJZoGIFUMg4QYCWRettUKu05QInFZK6V2dtast5RSkCOJ_jWQuVygVjL3hoCUOEbALKGVatOJgc1dKjWYFBdud5XzoW0WrgkomrLej7FYQo7Fhq56-pSRAWBhrNVOtxNZYNdT7War5QiMscACbYDIjG9xxIrXAlIhddVL8rV8stTyhNXTdxkTlWxHabE9p5rokG2SfqXgAB4BA1TDVyzVzLrKdpNvoDl9qKX1r5e4gAfK29trse2RyLWy3tzBgBTU5R2gtrDbW6m7Vak1ZrdRxgEOS4tq69DRBSPQegDqrnVgAKS2UrqA6uDyIBTmYPu6IAauVPpnY6qs25M08ofU84YryBAAGoHUlrmd4DQ9riGaifb0eNq67UBWkF0n4AgdJpAgAMtoQzuiYFGd0N9tFJk6RyphoEENqylDQNsAQEjyBAm1NYaJYFQh2HyNYTUzS_K8AOWON1FGQSTSmgAZh3kqO4YxcCYiNjNb5c6_mpkPGQQFbRgVFzBRCqFO9YUExJQi71Ag0UYuwFiid8JcMErGZgYlxQDMMqpSZ2lOK6JTtEhuwVc7-0ue5YywtHnZ2R2FdMfCora2-a_WMZ1S5Vj2hLuIKERMyIfN6FNVGRn0OYZBiCONVqtFGwNVyueEbv24hbW2-1-aD02pzHmSaFaq17V5aavMmRVbV2kTkl9qLBRKGYKipo3JrC9bM7l6rZBE2hBTS-yLfxc32rnqHBYW1K0KurUq0uFAkgzb5URw1DrI16oEHGErUXziVdcyum15rP0JtVfaED00LsRf82B1dpbU0NbWzWsbjL8ufv-6B114arVdodeyiN-p3CnodRJmAUmZMCGvSJ7TAVUN2A4roVxEhsMg2swR4ie2SPGI0Fj34oiBBGWuDETy7ZJEYeyh4-eTTJFLO8LQSZbWYUxCgN6MgxhYjCZsuJ-c8PpOXGsmJ0BPzFPKdU_hkFhtwXWUhVz91MQBC2dJd18J4QL5GepZivbuKcOEvw2brX9nKUG6c-F8HvbP3ssxr961_K3O4RC6KiYrJvCWSrHr13JcIOsDt5qgXRtNU415zofnQxt4CY69k4iOumgjYG0NkbxuW6U2UUPZk3h2x3F8IKBkfRJEWm1NcDpPmFhlGaZoMn7jC6gsEYCf2Ue-fh_9jsQ1bFQjq1cAaW4NoyKdcJ70WYkQTo-DfBBXw_su_V8NRhkk_4VhYWImX3wDftTk5HDXznNew9x8_eH47T2j-g4dwFplXnj-C5h5quHCPLjXpsku12xWrVn6bfq8zVXGVuQkYdBKIlJ0da8mxcdLM1ACdxkd5JkHANkVEWdfBellloDd4WY-MeYd5s14gXVgc60FN_kVMgVFdNMVdUd2sNdLcyVDM4MbcaUs9aI8V8cLc9M7M6CHNGCjcXcwd3d51ndL9xtHde1gsCJRUnAJUmxpVLIn1b1qC_wx8vVuDU9WA-t09ht1DRsD9W5c8yl-9C9XwMUyRmkK8dRtg1dtY-8C8-goRbRJ9PUt9LEUg-EtCaYe8uVD8QdxtJtk0aMzp4Ms0TliA7cv9fCbtf9x1nsHUgCfRQDkNxgXI0M4J7QOAoCzdYCidW4dIaw0jnCjBsp2MepsDZABM8DJoABOeTSOX5Eg-XdTFvZXAQVXBPGgjg7XQzQo3gASUnXfBRfCQ3bARzJg8zVgvDWAmzDoq3FFHg0zUPK_adG_J3D_DVK7N3RY02EVVhMVaQqVe0P3LLBNT1QIgQAAVgomVT2LVRdx32xyliGMmjuL30GJMysMTwERTzTyM0Gy0L62YIEEmX0PiDgEMLsOMNLzMINEr0sIE1VhsIH3-0cKTWcIwP9j5X9kiDEE408NdhyHmDZhnxDEKGaXuwdFmE1ntV3VQF5BWDAUb1ESpOOFYhROaVSPalxO1m8OXV8M9Wm0uk1TwLCL_AQxtTJIEBHWsiugAHYKsa94S-j7iddNVniBihi7cADMA4iQDb0UNki7ALA1IfAMi2CxlsjKYOxeQmY1YqxbRMluMjS1BD8dN2j4UuDrdjNRj7VxirM8NaCU8hjnMfC_soxJpDo3hWRMAAAxKMMiMhHoWyR6F3CMibV5AmCgYwMYMiNLF3NSbUD4ayOQTwboHmYMs2N8LSR0yaD5F3ZQhIss17d3cQ0LHYy4k485XoK6M4pMtopQpPFQj074poX4zPczSZLIOhCAFjZQ1EqsjALJT4iiQxAklIYIJROxUiUohbP8F6N6NiAQWgG_ZIys8Cf_S7HlY8v0cCerV6YaGImAZgI7aIHiR0v5EAXc4aAhGI93AHKMLVVYfpB8pQC6IInlPM94XUgCv8SWMiGkXyQ4PQSyR6WBE8GUElNAQo-4LuZQVQHeQ6LhesutNCBeD-cedyQEXHT-JnJbReMiyeFOAi1GMYroBBJBFBObeeIEBkOQO3WiieSaeMqwgcX0f0FaayKMowWZHeE8CwaYZwwYDoQJMSePVWOC5IXACXVteqAAHyjKlFTFTC-x3imGSCiBuDhHfkwAUqWUTSiCeW5HLRW0ayVV-CwonzSQ0oTJExsnVR401EsussCXaBC1vCJi-0VXaDQDcphHgs8t6BMrIDMtEAULohPFTB1Qjhwn6xWV-CUC4wiAwPRwfFARPDTQiFEAMSmGqTn0tH1MKEFF8E7mIB0WPXcj8u_DzmwHVTuCO2pgJl7W4jADZ1YCmmFSGB4p3jQORB-QhR6oZjaGjCVGYGqRgEdWMFTTmumlzVWJ6smj6sJkGtVIkFGqUHGsIVAUx36NERmpV02sOkWt8hWrWoCM2qmlSwolWIZ14xupaP2oGruCXOqR3EqT3TkG6IgBOrOsvnBpsjGufMIEBLAHBpEzhp4tWPZI4Fv1qIhT-sjkGrakxtOvho-p3isCbCxqypxp1X6rxrkFKHJqJrRqsJPCiCNJyWcItDgo42-VLjDIWv1EeveFWr9CMCJi-qwBWN6DIm8t6G8tRjwraECtcmCoIihBxzVogHVUOiVtwBVvwkAhuAUUGqQhwvcHFrMHOpN0TU7j1r4EPDQEwSJh7OkstBn031JNtMN1WF6FuCwUkQ4CUGEl7WMsDt9qNlxpwnxs9pMNBEZstrolrBtC9vwLpHILCqcu-xcqiqth3iBo0BBoFsjsunCvW0wBpGIFEHitDstmbPLtEEogBMTu5GTswEwS4gDorstilo0FzV8tEt4zbr9ibuTqlsukei1sVsPBsuiHWoSJdvDm41LwpFYTnFViqHtHwmAT2upuAXxp1FWuGz4AmtAXpqbE3tL2sj6t3rkEAlYF-h1EnkPuPtVjnj4uXntQhEvH3kBiPhPiwzPn2EvnlhvgRrkHEE7nwm1DLpCGfvfVIonhREvDNh1QllRF4vgeRE_qhBwECWSxzIE1QvQswt8DWANA2BpXE0wzsEsugMwHIb4UIp1nEG8hobN3odTXVQJuoYszYZM0YdSB0D5rxzw2OgAtYClH7OfXVWPPBqEdofYYsD-D0DnpKoEBdDdsYntEYgoAOG3AADUjBGBirVZwafBw5rJ-owp8JhpRpxod4rQbQhGnQ1A3RrQHKUr6ouEMLjAsKrg9YoJBR5l_hoDV66ILgmEjBls9y8LAl3JrIprWAyIol1VxbuIa9wbsqolegZHMMd4lzEpmcEyKq7AF80A2NMT25edZk9FXAChWZWQIgHAMChjvk_xwyoxzMolDBiByJDTwIkmfR5aCGBBBp64_GPhJZgJdRizfQUDnI-kPgDFCjywd4Zmu5YnJ5lmiYASVI5KMBsBGl7UgbQS5kQbDoTnIy8JKIzzZ4_wLmJtaErJLLpR5QbntYYMYi557nbUdkBZLKABpNiAATUihMiyFCiZ2-bbCefhH-fwjYheh0iQjYjedVg-flKIvz0jMecsgBeBdBfBdRcxahb5BhcOjheiCJc_2IpSGEr8qpf23gT9jkBdDsW3A7D0oMqMvjv215dc37qlibr4RZQFZLmuFwH4b5f23aoCqnqCrTNCrSaleVbohLqa1coTLUoQt8G0vhE5cMozviv0ESqZlEBiKlY1JVaBFFcHsRQFfwiFeGL3THqGate1gpVmQZcNSZcGtZaVFOoWQiC5uxNUVCtgbdcnXtcdZFeHDFbwElYjZ1gFaEZ1r1sVfNatbVazuiq1biprGNaSpEAzd5ctZVb8tbuMD9j8oddtL4VHt7uLbgUnsUuVpnoCNLf2zpeTesiWy7eHCsNVjbC8SNkOjbGbJmVmXIg8e1iSj0EFB4H1GqeaWPO6igE4wozGVCddi6Zk0FDteHHiujoZGndVhPBnKiVRMJS3e1i6brJPdSsVFFHWYWcqQOebBr3TReGsiHYoGInlzhcGhlDWCMjlHBV3R_ZyX_fwlTDYijNA-9I2b8LTQbRDTt0RhYqOwg7_fJcMiQh0hdDYlWJfppfmaCS1Wpm3F0XQ8o7JD0Cw3pq0iXJbV0gMmMjMgsDebJr9mGuFXrifUong2YcycGc-baYwY-F0VPoIi3oMSW3jIZak_Pp_hwdcgTZYMQ7MZ1Wi2o_OzhIffUYKk3zWnBu3PWggE0_xDedMe1VAmsms_Dl3UINdkHRI4wD9gFvyFWo8_tEogy0sfCiihigBNVlSYyZ0R9GyYrPBo7fs4yoseCisZsbGkigHYfcih6jyPamveI61Ci_I10SWzc7Im868-XBgF85aGKlKnKiC7eYxrIhyeymEeInC50HirSOE50HvfqkimmAsTzOMD30Wl7BWgyaZ2GoMCOcBFkfnJ9LUGgIG_FSJmGvC6KPeredfvE6Z3XpgCU7JFk4wnk8bZ2729BCWTU-sMVL3wGeyla47cuqVJW4EY7Y_P3Osle8eyc8ZcQ-1JUcNRkp_GKyE6CDZmaQyc5NViBpm9g1N2syGMW6iBu9MEE6bGyreumkuKHeudE_hCot0RO5k7sDk63gZYJ4ZBU4lfu6u6NvBru5iI-_e9vP3KB1S_qlksKT_Fka4ZB7mZ46m4-AJrOdh7wwW7EB9CW4GQ2fa6y_W5x7fok7JDJ5_iKCJ8O5J-O_3tO4p4u4VIZKwye-SZiIe-u4Jrp4xfU4Wa1OAL-65RZv1EygdN4BUq5X2EOEmi6eIHt_3f8nQasrleVrrNd9wG64KYNucPy31E3wYxumiFM0wEy1X2BIEBuiMgAC0rgPgbpwTCgNFvxS5QR7UHHuRbV7CyIbpp3NvlUJ4xjxPEHsGDYCRGlsyaoW-J6S_nRhsuJzlW-KE9kupml4kNQkk5E6lfxjh65UF_hinrWugbhUJNd8JoB4B4YYW5B4Yz58I5BYEYK2_pIuIKIwBY4MYgA
---

# Pygame

- Out of the box
- No sound
- Some issues
- Solid Basis for GameGrid

---
layout: center
---

# In Progress Projects

---

# Robotics Simulation - Microbit

<video width="1080" controls>
  <source src="./images/LabyrinthLoadEnvironement.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

# Robotics Simulation - Calliope

<video width="1080" controls>
  <source src="./images/CallibotFollowTheLine.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

# JythonMusic

---

# Databases

![](./images/database1.png)

---

# Databases

![](./images/database2.png)

---

# Databases
![](./images/database3.png)

---

# Databases
![](./images/database4.png)