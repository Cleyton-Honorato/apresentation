<script setup lang="ts">
withDefaults(
  defineProps<{
    /** Variante do logo: completo ou apenas o símbolo "A" */
    variant?:
      | 'full-white'
      | 'full'
      | 'full-black'
      | 'a-white'
      | 'a-purple'
      | 'a-black'
  }>(),
  { variant: 'full-white' },
)

const files: Record<string, string> = {
  'full-white': '/logos/academe-full-white.svg',
  'full': '/logos/academe-full.svg',
  'full-black': '/logos/academe-full-black.svg',
  'a-white': '/logos/academe-a-white.svg',
  'a-purple': '/logos/academe-a-purple.svg',
  'a-black': '/logos/academe-a-black.svg',
}
</script>

<template>
  <img :src="files[variant]" alt="Academe" />
</template>
