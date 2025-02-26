<script setup>
import { ref } from 'vue'
import { useRouter } from 'vue-router'

const router = useRouter()

const goToAbout = () => {
  router.push('/HomeView')
}

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
    <div class="min-h-screen flex flex-col justify-center items-center text-center">
      <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded cursor-pointer" @click="goToAbout">Go to Page HomeView</button>
      <h1>{{ msg }}</h1>
      <div class="card">
        <button type="button" @click="count++">count is {{ count }}</button>
        <p>
          Edit
          <code>components/HelloWorld.vue</code> to test HMR
        </p>
      </div>

      <p>
        Check out
        <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank">create-vue</a>, the official Vue + Vite
        starter
      </p>
      <p>
        Learn more about IDE Support for Vue in the
        <a href="https://vuejs.org/guide/scaling-up/tooling.html#ide-support" target="_blank">Vue Docs Scaling up
          Guide</a>.
      </p>
      <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
    </div>

</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
