---
layout: image
image: /background-list.jpg
transition: fade-out
title: Non Null Assertion
---

<div class="flex flex-justify-center h-full flex-col">
  <div class="background">

  <h1 class="text-left m-b-0 font-bold">
    # Non Null Assertion
  </h1>

```js {all|1|6|1|2|3|8|1|2|3|all} {lines:true} twoslash
const greetUser = (name: string | null): void => {
  const formattedName: string = name!;
  console.log(`Hello, ${formattedName || 'Geeks'}!`);
}

greetUser("Akshit");

greetUser(null);
```

  </div>
</div>
<!-- name santi020k -->
