<script lang="ts">
import { defineComponent, ref } from 'vue' // Cannot resolve symbol 'defineComponent / ref'
export default defineComponent({
  setup() {
    const devMode = ref(import.meta.env.DEV)

    return {
      devMode,
    }
  },
})
</script>

<template>
  {{ devMode }}

  <RouterView />
</template>
