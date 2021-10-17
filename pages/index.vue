<template>
  <div class="flex flex-row h-screen">
    <div class="hidden w-1/3 md:flex items-center justify-center h-full">
      <h1>
        <img src="~/assets/logo.svg" width="150" height="53" alt="CBFN" />
      </h1>
    </div>
    <div
      class="w-full md:w-2/3 bg-white h-full flex flex-col p-8 justify-center"
    >
      <h1 class="block md:hidden mb-8">
        <img src="~/assets/logo-dark.svg" width="150" height="53" alt="CBFN" />
      </h1>
      <h2 class="text-5xl">Web</h2>
      <h2 class="text-5xl">Mobile</h2>
      <h2 class="text-5xl">Support</h2>
      <h2 class="text-5xl">& Company Training</h2>
      <div class="space-x-2 text-2xl mt-8">
        <a
          href="https://www.instagram.com/cbfn.dev/"
          title="Follow me on instagram"
          class="
            border border-purple-700
            text-purple-700
            hover:bg-purple-700 hover:text-white
            rounded-full
            transition-all
            duration-500
            ease-in-out
            py-4
            px-8
          "
          >Follow me on <font-awesome-icon :icon="['fab', 'instagram']"
        /></a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  head() {
    return {
      title: 'Web, Mobile, Support Development & Company Training | CBFN',
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'description',
          name: 'description',
          content:
            'We create web and mobile applications that helps companies to generate more results for their customers.',
        },
      ],
    }
  },
})
</script>

<style>
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
  font-weight: 300;
}
.title > span {
  font-size: 60px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #f9f9f9;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
