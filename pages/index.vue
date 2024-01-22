<script setup lang="ts">
  const online = useOnline()
  useSeoMeta({
    title: 'QuickCook app',
    description: 'QuickCook is small app to help you cook.',
  })

  defineOgImage({
    title: 'QuickCook app',
    description: 'QuickCook is small app to help you cook.',
  })
</script>

<template>
  <Home />
</template>
