<template>
  <div class="home">
    <input type="color" v-model="btn.background" />
    <label for="width">Width</label>
    <input id="width" type="text" v-model="btn.width" />
    <label for="height">Height</label>
    <input id="height" type="text" v-model="btn.height" />
    <label for="fontSize">Font Size</label>
    <input id="fontSize" type="text" v-model="btn.fontSize" />
    <label for="fontFamily">Font Family</label>
    <input id="fontFamily" type="text" v-model="btn.fontFamily" />
    {{ btn.background }}
    <a :style="btn" href="">Clique aqui</a>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  data() {
    return {
      btn: {
        background: "#000",
        width: "100px",
        height: "40px",
        fontSize: "12px",
        fontFamily: "monospace",
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
  margin-top: 100px;
}
</style>
