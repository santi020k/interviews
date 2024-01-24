<template>
  <div class="box-model">
    <div class="margin">
      <div class="border">
        <div class="padding">
          <div class="content" />
        </div>
      </div>
    </div>
  </div>

  <component :is="'style'">
    .box-model {
      max-width: 500px;
    }

    .margin {
      background: #f1f1f1;
      padding: 45px;
      width: 100%;
      height: 100%;
      position: relative;
      border: 2px dashed #bbb;
      transition: all .25s ease-in-out;
      color: black;
    }

    .margin:before {
      content: "Margin";
      font-size: 1.4em;
      position: absolute;
      left: 0;
      top: 1.8%;
      width: 100%;
      text-align: center;
    }

    .border {
      padding: 45px;
      width: 100%;
      height: 100%;
      position: relative;
      color: #fff;
      background-color: #04AA6D;
    }

    .border:before {
      content: "Border";
      font-size: 1.4em;
      color: black;
      position: absolute;
      left: 0;
      top: 2.5%;
      width: 100%;
      text-align: center;
    }

    .padding {
      color: black;
      padding: 45px;
      width: 100%;
      height: 100%;
      position: relative;
      background: #f1f1f1;
    }

    .padding:before {
      content: "Padding";
      font-size: 1.4em;
      position: absolute;
      left: 0.5%;
      top: 3.7%;
      width: 100%;
      text-align: center;
    }

    .content {
      padding: 20px;
      width: 100%;
      height: 100%;
      position: relative;
      background: white;
      border: 2px dashed #bbb;
    }

    .content:before {
      content: "Content";
      font-size: 1.4em;
      display: block;
      text-align: center;
      line-height: 3.5;
    }
  </component>
</template>
