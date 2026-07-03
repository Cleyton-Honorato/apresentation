<script setup lang="ts">
defineProps<{
  /** Texto opcional à esquerda do rodapé */
  label?: string
}>()
</script>

<template>
  <div class="absolute bottom-4 left-6 right-6 flex items-center justify-between text-xs opacity-60">
    <span>{{ label ?? '' }}</span>
    <AcademeLogo variant="full-black" class="h-4" />
  </div>
</template>
