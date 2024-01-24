---
layout: image
image: /background-list.jpg
transition: fade-out
title: Solution Specificity
---

<div class="flex flex-justify-center h-full flex-col">
  <div class="background">

  <h1 class="text-left m-b-0 font-bold">
    # Specificity
  </h1>

```html {all} {lines:true}
  <div id="id-example" class="class-example" />
```

```css {all} {lines:true}
  * { /* 0-0-0 */
    backgroundColor: "red";
  }

  div { /* 0-0-1 */
    backgroundColor: "yellow";
  }

  .class-example { /* 0-1-0 */
    backgroundColor: "green";
  }

  #id-example { /* 1-0-0 */
    backgroundColor: "blue";
  }
```

  </div>
</div>
<!-- Y Error -->
