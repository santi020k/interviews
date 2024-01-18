---
layout: image
image: /background-list.jpg
transition: fade-out
title: Optional Chaining
---

<div class="flex flex-justify-center h-full flex-col">
  <div class="background">

  <h1 class="text-left m-b-0 font-bold">
    # Optional Chaining
  </h1>

```js {all|1|8|10|12|14|all} {lines:true} twoslash
  const adventurer = {
    name: 'Alice',
    cat: {
      name: 'Dinah',
    },
  };

  const dogName = adventurer.dog?.name;

  console.log(dogName);

  console.log(adventurer.someNonExistentMethod?.());

  console.log(adventurer.cats?.[0]);
```

  </div>
</div>
<!-- name santi020k -->
