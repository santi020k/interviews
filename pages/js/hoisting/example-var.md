---
layout: image
image: /background-list.jpg
transition: fade-out
title: Hoisting Example
---

<div class="flex flex-justify-center h-full flex-col">
  <div class="background">

  <h1 class="text-left m-b-0 font-bold">
    # Hoisting Example
  </h1>

```ts {all|1|2|3|all} {lines:true} twoslash
  var x: number = 5;
  console.log(`'x' is  = ${ x }, 'y' is = ${ y }`);
  //                                         ^?
  var y: number = 7;
```

  </div>
</div>
<!-- Y undefined -->
