<template>
  <img v-bind:src="url" alt="" />
  <!-- <img :src="url" alt="" /> -->

  <button v-bind:disabled="isDisabled">Click me</button>

  <button v-bind:disabled="isDisabled"></button>

  <input type="text" v-bind:disabled="isEnter" />

  <div v-bind="divAttributes">Container</div>

  <!-- Binding 2 thuộc tính id: "paragraph", area="paragrrap" -->
  <p v-bind="paragraphAttributes">Nội dung</p>

  <!-- v-bind cho class và style -->
  <div v-bind:class="{ textRed: isTextRed }">Hello world</div>
</template>

<script setup>
const url =
  "https://www.vietnamworks.com/hrinsider/wp-content/uploads/2023/12/hinh-anh-thien-nhien-dep-3d-001.jpg";

const isDisabled = true;

const isEnter = true;

const divAttributes = {
  id: "container-id",
  class: "container-class",
};

const paragraphAttributes = {
  id: "paragraph",
  area: "paragraph",
};

const isTextRed = true;
</script>

<style>
.textRed {
  color: red;
}
</style>
