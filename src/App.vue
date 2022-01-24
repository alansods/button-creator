<template>
  <div id="app">
    <div class="home">
      <label for="background">Background Color</label>
      <input type="color" v-model="btn.background" />
      {{ btn.background }}
      <label for="color">Color</label>
      <input type="color" v-model="btn.color" />
      {{ btn.color }}
      <label for="width">Width</label>
      <input id="width" type="text" v-model="btn.width" />
      <label for="height">Height</label>
      <input id="height" type="text" v-model="btn.height" />
      <label for="fontSize">Font Size</label>
      <input id="fontSize" type="text" v-model="btn.fontSize" />
      <label for="fontWeight">Font Weight</label>
      <input id="fontWeight" type="text" v-model="btn.fontWeight" />
      <label for="fontFamily">Font Family</label>
      <input id="fontFamily" type="text" v-model="btn.fontFamily" />
      <label for="textAlign">Text Align</label>
      <input id="textAlign" type="text" v-model="btn.textAlign" />
      <label for="borderRadius">Border Radius</label>
      <input id="borderRadius" type="text" v-model="btn.borderRadius" />
      <a :style="btn" href="">Clique aqui</a>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      btn: {
        background: "#0065B3",
        color: "#ffffff",
        width: "120px",
        height: "40px",
        fontSize: "14px",
        fontFamily: "arial",
        textAlign: "center",
        borderRadius: "20px",
        fontWeight: "bold",
        display: "flex",
        alignItems: "center",
        justifyContent: "center",
        textDecoration: "none",
      },
    };
  },
};
</script>

<style>
label {
  display: block;
}

a {
  display: block;
  margin-top: 2
  0px;
}
</style>
