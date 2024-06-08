<script setup lang="ts">
import { onMounted } from 'vue'
import { useRouter } from 'vue-router'
const router = useRouter()
onMounted(() => {
  console.log('App.vue mounted')
  router.replace('/')
})
</script>

<template>
  <Suspense>
    <RouterView />
  </Suspense>
</template>

<style></style>
