---
layout: image
image: /background-list.jpg
transition: fade-out
title: The Event Loop Example Code
---

<div class="flex flex-justify-center h-full flex-col">
  <div class="background">

  <h1 class="text-left m-b-0 font-bold">
    # The Event Loop
  </h1>

```ts {all|1|5|9|1|2|10|5|6|all} {lines:true} twoslash
const greet = () => {
  return 'Hello';
}

const respond = () => {
  return setTimeout(() => 'Hey!', 1000)
}

greet();
respond();
```

  </div>
</div>
