<template>
  <div class="flex items-center justify-between gap-4 py-4 <sm:flex-col">
    <div class="text-hint">rtx3.com
    </div>
    <div class="flex items-center gap-4">
      <DarkToggle />
      <LangToggle />
      <a
        href="https://rtx3.com"
        target="_blank"
        class="i-logos-webhooks cursor-pointer text-lg"
      ></a>
    </div>
  </div>
</template>
<script lang="ts" setup>
  const Author = 'rtx3'
</script>
