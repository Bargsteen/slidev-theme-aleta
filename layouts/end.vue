<script setup lang="ts">
import { computed } from 'vue'
import { handleBackground } from '../layoutHelper'

const props = defineProps({
  background: {
    default: '',
  },
})

const style = computed(() => handleBackground(props.background, true))
</script>

<template>
  <div class="slidev-layout end">
    <img class="aleta-logo" src="../public/logo-tagline.black.png" />
  </div>
</template>
