<template>
  <div class="container">
    <div id="heart">
      <div class="item item-opacity"></div>
      <div class="item drop-animation5"></div>
      <div class="item drop-animation3"></div>
      <div class="item item-opacity"></div>
      <div class="item drop-animation4"></div>
      <div class="item drop-animation2"></div>
      <div class="item item-opacity"></div>

      <div class="item drop-animation4"></div>
      <div class="item drop-animation2"></div>
      <div class="item drop-animation1"></div>
      <div class="item drop-animation4"></div>
      <div class="item drop-animation1"></div>
      <div class="item drop-animation3"></div>
      <div class="item drop-animation5"></div>

      <div class="item drop-animation2"></div>
      <div class="item drop-animation4"></div>
      <div class="item drop-animation1"></div>
      <div class="item drop-animation3"></div>
      <div class="item drop-animation5"></div>
      <div class="item drop-animation4"></div>
      <div class="item drop-animation1"></div>

      <div class="item drop-animation3"></div>
      <div class="item drop-animation4"></div>
      <div class="item drop-animation1"></div>
      <div class="item drop-animation3"></div>
      <div class="item drop-animation3"></div>
      <div class="item drop-animation1"></div>
      <div class="item drop-animation5"></div>

      <div class="item item-opacity">1</div>
      <div class="item drop-animation1"></div>
      <div class="item drop-animation2"></div>
      <div class="item drop-animation1"></div>
      <div class="item drop-animation4"></div>
      <div class="item drop-animation2"></div>
      <div class="item item-opacity"></div>

      <div class="item item-opacity"></div>
      <div class="item item-opacity"></div>
      <div class="item drop-animation1"></div>
      <div class="item drop-animation5"></div>
      <div class="item drop-animation3"></div>
      <div class="item item-opacity"></div>
      <div class="item item-opacity"></div>

      <div class="item item-opacity"></div>
      <div class="item item-opacity"></div>
      <div class="item item-opacity"></div>
      <div class="item drop-animation4"></div>
      <div class="item item-opacity"></div>
      <div class="item item-opacity"></div>
      <div class="item item-opacity"></div>
    </div>
    <p id="i">520 又到啦，今年送什么给我的佳佳老婆呢？</p>
    <p id="love">想了好久，最终小脑瓜灵光一闪！这个小页面做出来啦~</p>
    <p id="you">虽然很简单，但是就像老公对你的爱，永远都是粉色哒</p>
    <p id="gift">至于礼物嘛，微信上给老公发“爱你哟”试试看~</p>
  </div>
</template>

<script>
export default {
  name: "Index",
  props: {
    text: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
#heart {
  display: grid;
  width: 80%;
  height: 80vw;
  padding: 10%;
  grid-template-columns: repeat(7, 1fr);
  grid-template-rows: repeat(7, 1fr);
  grid-row-gap: 0.5%;
  grid-column-gap: 1%;

  .item {
    background-color: #ffffff;
    border-radius: 10%;

    &.drop-animation1 {
      transform: translateY(-600px);
      opacity: 0;
      animation: drop-down1 5s ease-in-out 1s infinite normal running forwards;
    }

    &.drop-animation2 {
      transform: translateY(-800px);
      opacity: 0;
      animation: drop-down2 5s ease-in-out 1s infinite normal running forwards;
    }

    &.drop-animation3 {
      transform: translateY(-1000px);
      opacity: 0;
      animation: drop-down3 5s ease-in-out 1s infinite normal running forwards;
    }

    &.drop-animation4 {
      transform: translateY(-1200px);
      opacity: 0;
      animation: drop-down4 5s ease-in-out 1s infinite normal running forwards;
    }

    &.drop-animation5 {
      transform: translateY(-1400px);
      opacity: 0;
      animation: drop-down5 5s ease-in-out 1s infinite normal running forwards;
    }
  }

  .item-opacity {
    opacity: 0;
  }
}
#i {
  margin: 5%;
  margin-top: 25%;
  color: #ffffff;
  font-size: 14px;
  font-family: "MicroSoft Yahei";
  white-space: nowrap;
  border-right: 2px solid transparent;
  opacity: 0;
  animation: typing1 3s steps(20, end) 1s forwards, blink-caret 0.75s step-end 5;
  overflow: hidden;
}
#love {
  margin: 5%;
  color: #ffffff;
  font-size: 14px;
  font-family: "MicroSoft Yahei";
  white-space: nowrap;
  border-right: 2px solid transparent;
  opacity: 0;
  animation: typing2 3s steps(25, end) 4s forwards, blink-caret 0.75s step-end 9;
  overflow: hidden;
}
#you {
  margin: 5%;
  color: #ffffff;
  font-size: 14px;
  font-family: "MicroSoft Yahei";
  white-space: nowrap;
  border-right: 2px solid transparent;
  opacity: 0;
  animation: typing3 3s steps(24, end) 7s forwards, blink-caret 0.75s step-end 13;
  overflow: hidden;
}
#gift {
  margin: 5%;
  color: #ffffff;
  font-size: 14px;
  font-family: "MicroSoft Yahei";
  white-space: nowrap;
  border-right: 2px solid transparent;
  opacity: 0;
  animation: typing4 3s steps(21, end) 10s forwards, blink-caret 0.75s step-end infinite;
  overflow: hidden;
}

/* 各种 dropDown */
@keyframes drop-down1 {
  20%,
  80% {
    transform: translateY(0);
    opacity: 1;
  }
  100% {
    transform: translateY(1400px);
    opacity: 0;
  }
}
@keyframes drop-down2 {
  20%,
  80% {
    transform: translateY(0);
    opacity: 1;
  }
  100% {
    transform: translateY(1200px);
    opacity: 0;
  }
}
@keyframes drop-down3 {
  20%,
  80% {
    transform: translateY(0);
    opacity: 1;
  }
  100% {
    transform: translateY(1000px);
    opacity: 0;
  }
}
@keyframes drop-down4 {
  20%,
  80% {
    transform: translateY(0);
    opacity: 1;
  }
  100% {
    transform: translateY(800px);
    opacity: 0;
  }
}
@keyframes drop-down5 {
  20%,
  80% {
    transform: translateY(0);
    opacity: 1;
  }
  100% {
    transform: translateY(600px);
    opacity: 0;
  }
}
/* 打印效果 */
@keyframes typing1 {
  from {
    width: 0;
    opacity: 1;
  }
  to {
    width: 20em;
    opacity: 1;
  }
}
@keyframes typing2 {
  from {
    width: 0;
    opacity: 1;
  }
  to {
    width: 25em;
    opacity: 1;
  }
}
@keyframes typing3 {
  from {
    width: 0;
    opacity: 1;
  }
  to {
    width: 24em;
    opacity: 1;
  }
}
@keyframes typing4 {
  from {
    width: 0;
    opacity: 1;
  }
  to {
    width: 21em;
    opacity: 1;
  }
}
/* 光标闪啊闪 */
@keyframes blink-caret {
  from,
  to {
    box-shadow: 1px 0 0 0 transparent;
  }
  50% {
    box-shadow: 1px 0 0 0;
  }
}
</style>
