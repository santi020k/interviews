---
layout: image
image: /background-list.jpg
transition: fade-out
title: Closure Example
---

<div class="flex flex-justify-center h-full flex-col">
  <div class="background">

  <h1 class="text-left m-b-0 font-bold">
    # Closure Example
  </h1>

```ts {all|1|9|1|2|3|6|3|4|all} {lines:true} twoslash
  const init = (): void => {
    const name: string = "santi020k";
    const displayName = (): void => {
      console.log(name);
      //           ^?
    }
    displayName();
  }

  init();
```

  </div>
</div>
<!-- name santi020k -->
