/* eslint-disable quotes */
<template>
  <div>
    <div class="container">
      <div>
        <logo />
        <h1 class="title">first-nuxt-app</h1>
        <h2 class="subtitle">My laudable Nuxt.js project</h2>

        <div class="links">
          <button
            class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-full"
          >
            Button
          </button>
          <a href="https://nuxtjs.org/" target="_blank" class="button--green"
            >Documentation</a
          >
          <a
            href="https://github.com/nuxt/nuxt.js"
            target="_blank"
            class="button--grey"
            >GitHub</a
          >
        </div>
      </div>
    </div>
    <div class="mx-auto px-2 bg-indigo-300 h-64">
      <button
        class="mt-5 bg-blue-500 hover:bg-blue-700 text-white font-extrabold py-2 px-4 rounded-full"
      >
        hello world
      </button>
      <div
        class="bg-red-100 border border-red-400 text-red-700 px-4 py-3 rounded relative my-5"
        role="alert"
      >
        <strong class="font-bold">ALERT!</strong>
        <span class="block sm:inline">Please update your password</span>
      </div>

      <div
        class="max-w-sm mx-auto flex p-6 bg-white rounded-lg shadow-xl"
      ></div>
    </div>
    <button
      :class="[]"
      class="bg-blue-500 text-white font-bold py-2 px-4 border border-blue-700 rounded inline-flex items-center hover:bg-blue-600"
    >
      TESTING
    </button>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo
  },
  data() {
    return {
      message: "helloworld wtf bbq sauce"
    };
  }
};
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
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
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
