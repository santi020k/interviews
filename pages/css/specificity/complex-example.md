---
layout: image
image: /background-list.jpg
transition: fade-out
title: Complex examples Specificity
---

<div class="flex flex-justify-center h-full flex-col">
  <div class="background">

  <h1 class="text-left m-b-0 font-bold">
    # Specificity
  </h1>

```css {all} {lines:true}
  [type="password"]             /* 0-1-0 */
  input:focus                   /* 0-1-1 */
  :root #myApp input:required   /* 1-2-1 */
  :is(p)                        /* 0-0-1 */
  h2:nth-last-of-type(n + 2)    /* 0-1-1 */
  h2:has(~ h2)                  /* 0-0-2 */
  div.outer p                   /* 0-1-2 */
  div:not(.inner) p             /* 0-1-2 */
```

  </div>
</div>
<!-- Y Error -->
