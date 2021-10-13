<template>
  <div class="maincontainer">
    <div
      style="width: 800px; height: 604px; margin-left: 25px; margin-top: 20px"
      id="widget"
    >
      <img
        src="./assets/bartback.png"
        style="width: 800px; height: 604px; position: absolute; z-index: 0"
      />
      <section
        id="chalk"
        class="container"
        style="position: absolute; z-index: 1"
      >
        <div class="box" id="theBox" style="font-size: 18px">
          {{ message }}
        </div>
      </section>
      <img
        src="./assets/bartfront.png"
        style="width: 800px; height: 604px; position: absolute; z-index: 2"
      />
    </div>
    <div
      style="
        margin-left: 25px;
        width: 760px;
        position: relative;
        z-index: 2;
        background: #fff;
        padding: 20px;
      "
    >
      <textarea v-model="message" style="width: 350px; height: 260px">
      </textarea>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    message: `
      
  ottos mops
  ottos mops trotzt
  otto: fort mops fort
  ottos mops hopst fort
  otto: soso
  otto holt koks
  otto holt obst
  otto horcht
  otto: mops mops
  otto hofft
  ottos mops klopft
  otto: komm mops komm
  ottos mops kommt
  ottos mops kotzt
  otto: ogottogott`,
  }),
};
</script>

<style>
#app {
  font-family: "./assets/djb_chalk_it_upregular";
  font-family: "djb_chalk_it_upregular";
  background-color: #9bdcfa;
}

@font-face {
  font-family: "./assets/djb_chalk_it_upregular";

  src: url("./assets/djb_chalk_it_up-webfont.eot");

  src: url("./assets/djb_chalk_it_up-webfont.eot?#iefix")
      format("embedded-opentype"),
    url("./assets/djb_chalk_it_up-webfont.woff2") format("woff2"),
    url("./assets/djb_chalk_it_up-webfont.woff") format("woff"),
    url("./assets/djb_chalk_it_up-webfont.ttf") format("truetype"),
    url("./assets/djb_chalk_it_up-webfont.svg#djb_chalk_it_upregular")
      format("svg");

  font-weight: normal;

  font-style: normal;
}

.container {
  width: 410px;
  height: 400px;
}

.maincontainer {
  position: absolute;
  width: 850px;
  height: auto;
  left: 50%;
  margin-left: -425px;
  background: #fff;
  border-radius: 10px 10px 10px 10px;
  -moz-border-radius: 10px 10px 10px 10px;
  -webkit-border-radius: 10px 10px 10px 10px;
  border: 0px solid #adadad;
}

.mytext {
  width: 850px;
  height: auto;
  left: 50%;
}

.box {
  width: 100%;
  height: 100%;
  word-wrap: normal;
  text-wrap: normal;
  line-height: 19px;
  overflow: hidden;
  text-overflow: ellipsis;
  margin-left: 120px;
  white-space: pre;
}

#chalk {
  -webkit-perspective: 800px;
  -moz-perspective: 800px;
  -o-perspective: 800px;
  perspective: 800px;

  -webkit-perspective-origin: 50% 65%;
  -moz-perspective-origin: 50% 65%;
  -o-perspective-origin: 50% 65%;
  perspective-origin: 50% 65%;
}

#chalk .box {
  color: white;
  font-size: 25px;
  font-family: "djb_chalk_it_upregular";
  -webkit-transform: rotateY(35deg);
  -moz-transform: rotateY(35deg);
  -o-transform: rotateY(35deg);
  transform: rotateY(35deg);
}
</style>
