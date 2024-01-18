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

```ts {all|3|12|3|4|5|8|9|12|14|5|6|all} {lines:true} twoslash
type VFunction = () => void;

const numberGenerator = (): VFunction => {
  let number: number = 1;
  function checkNumber() {
    console.log(number);
    //            ^?
  }
  number =+ 1;
  return checkNumber;
}

const printNumber: VFunction = numberGenerator();

printNumber();
```

  </div>
</div>
<!-- Print 2 -->
