---
# config for the whole slides and the first one

addons:
  - slidev-addon-python-runner
  - slidev-addon-rabbit
rabbit:
  slideNum: true   # Show current/total slide numbers next to a rabbit icon

theme: bricks

# some information about your slides (markdown enabled)
title: Property Management
author: Siddarth Datla
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false

# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left

# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true

# show line numbers in code blocks
lineNumbers: True

# controls whether texts in slides are selectable
selectable: true
---

# Property Management

A Changing Paradigm

<div class="abs-br m-6 text-xl">
  <a href="https://www.youtube.com/@KareemKreates" target="_blank" class="slidev-icon-btn">
    <carbon:logo-youtube />
  </a>
  <a href="https://github.com/KareimGazer" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
    <a href="https://x.com/KareimGazer" target="_blank" class="slidev-icon-btn">
    <carbon:logo-x />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
src: ./pages/toc.md
---

---
src: ./pages/why.md
---

---
src: ./pages/philosophy.md
---

---
src: ./pages/pillar-one.md
---

---
src: ./pages/pillar-two.md
---

---
src: ./pages/pillar-three.md
---

---
src: ./pages/pain-points.md
---

---
src: ./pages/intro.md
---

---
src: ./pages/market-shift.md
---

---
src: ./pages/our-solution.md
---

---
src: ./pages/implementation.md
---

---
src: ./pages/call-to-action.md
---

---
layout: center
class: text-center
---

# Learn More

[Materials](https://sli.dev) · [GitHub](https://github.com/KareimGazer) · [YouTube](https://www.youtube.com/@KareemKreates)

<PoweredBySlidev mt-10 />
