---
layout: image
image: /background-list.jpg
transition: fade-out
title: The Event Loop Complex Example Code
---

<div class="flex flex-justify-center h-full flex-col">
  <div class="background">

  <h1 class="text-left m-b-0 font-bold">
    # The Event Loop
  </h1>

```ts {all|1|11|7-9|3-5|all} {lines:true} twoslash
console.log('Start');

setTimeout(() => {
 console.log('setTimeout Callback');
}, 0);

Promise.resolve().then(() => {
 console.log('Promise Resolved');
});

console.log('End');
```

  </div>
</div>
