<script setup>
  const props = defineProps({
    stringProp: String
  })

  const emit = defineEmits(
    [
      'buttonEmit'
    ]
  )

  let nonReactivePayload = 50

</script>

<template>
  <div>
    <button class="bg-purple-700 px-5 py-2 rounded-md text-white font-semibold text-lg hover:bg-purple-600" @click="emit('buttonEmit', nonReactivePayload)">Click me</button>
  </div>
</template>

<style scoped>

</style>