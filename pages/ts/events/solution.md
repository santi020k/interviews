---
layout: image
image: /background-list.jpg
transition: fade-out
title: Type Events in React with TypeScript
---

<div class="flex flex-justify-center h-full flex-col">
  <div class="background">

  <h1 class="text-left m-b-0 font-bold">
    # Type Events in React with TypeScript
  </h1>

```tsx {all} {lines:true} twoslash
// ✅ Correct way
const handleClick = (event: React.MouseEvent<HTMLButtonElement>) => {
    console.log('click', event);
 };

 // ❌ Junior way
const handleClick = (event: any | unknown) => {
    console.log('click', event);
 };

 // ❌ Mid way
const handleClick = (event: Record<string, string>) => {
    console.log('click', event);
 };
```

  </div>
</div>
<!-- name santi020k -->
