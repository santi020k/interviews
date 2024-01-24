---
layout: image
image: /background-list.jpg
transition: fade-out
title: Example Specificity
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
  * {
    backgroundColor: "red";
  }

  div {
    backgroundColor: "yellow";
  }

  .class-example {
    backgroundColor: "green";
  }

  #id-example {
    backgroundColor: "blue";
  }
```

  </div>
</div>
