<template>
  <div class="app">
    <h1>{{title}}</h1>
    <input class="input" type="text" v-model="text" placeholder="digite para gerar..." />
    <div v-if="text" class="output">
      <img alt="QrCode" :src="newQrCode" />
    </div>
  </div>
</template>

<script>
import Qrious from "qrious";
export default {
  data() {
    return {
      text: "http://www.google.com.br",
      title: "Gerador de QrCode",
      qrcode: new Qrious({
        size: 300
      })
    };
  },
  computed: {
    newQrCode() {
      return this.setTextOnValue(this.text);
    }
  },
  methods: {
    setTextOnValue(text) {
      this.qrcode.value = text;
      return this.qrcode.toDataURL();
    }
  }
};
</script>

<style>
</style>