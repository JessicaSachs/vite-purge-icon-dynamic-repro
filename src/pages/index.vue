<script lang="ts">
import '@iconify/iconify'
import '@purge-icons/generated'

import { defineComponent } from 'vue'
export default defineComponent({
  setup() {
    return {
      show: ref(false)
    }
  }
})
</script>

<template>
  <div class="w-400px text-center mx-auto my-0">
    <p>Click <a class="underline text-indigo-500" @click="show = !show">here</a> to toggle the heart icon.</p>
    <p>Showing? {{ show }} <i :data-icon="show ? 'mdi:heart' : 'mdi:heart-broken'" class="iconify text-red-500" /></p>
  </div>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
