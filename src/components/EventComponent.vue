<script setup>
const handleClick = () => {
  console.log("Clicked");
};

const handleDetele = (id) => {
  console.log("Id: ", id);
};

const handleGetEvent = (event) => {
  console.log("Event: ", event);
};

const handleSubmit = () => {
  alert("Submited");
};

// Được kích hoạt khi người dùng nhấn vào nút "Đóng form" hoặc nhấn phím 'esc'
const handleCloseForm = () => {
  alert("Đóng Form");
};
</script>

<template>
  <button v-on:click="handleClick">Click me</button>
  <button v-on:click="handleDetele(1)">Delete</button>
  <button @click="handleGetEvent">Event info</button>

  <form @submit.prevent="handleSubmit">
    <button type="submit">Submit</button>
  </form>

  <button @keydown.esc="handleCloseForm">Đóng form</button>
</template>

<style></style>
