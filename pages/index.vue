<template>
  <div class="container mx-auto px-4 flex flex-col">
    <h1 class="title"><span>&lt;</span>BFN</h1>
    <h2>Web, Mobile and Support Development | Company Training</h2>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300&display=swap');
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Inter', sans-serif;
  display: block;
  @apply font-bold;
  font-size: 80px;
  color: #35495e;
  letter-spacing: 1px;
}
.title > span {
  @apply font-bold;
  font-size: 100px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
