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
      <h2 class="text-2xl mb-4">About CBFN</h2>
      <p>
        CBFN is a small company specialized in web, mobile, IT support and
        consulting for startups, small, medium and big companies based on
        Florianópolis, SC, Brazil.
      </p>
      <h2 class="my-4 text-2xl">Address</h2>
      <address>
        Rua Sebastião Laurentino da Silva, 170, Apt 101<br />CEP 88037-400,
        Florianópolis, SC, Brazil
      </address>
      <footer class="mt-12">
        <small
          >This site is owned and operated by Christian Barros Fabião do
          Nascimento</small
        >
      </footer>
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
            'CBFN is a small company specialized in web, mobile, it support and consulting for startups, small, medium and big companies based on Florianópolis, SC, Brazil.',
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
