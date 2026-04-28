<script setup lang="ts">
type KeywordSize = 'sm' | 'md' | 'lg'

// biome-ignore lint/correctness/noUnusedVariables: props are used in template
const props = withDefaults(
  defineProps<{
    size?: KeywordSize
  }>(),
  { size: 'md' }
)
</script>

<template>
  <span class="slidev-keyword" :class="[`slidev-keyword--${props.size}`]">
    <slot />
  </span>
</template>

<style scoped>
.slidev-keyword {
  color: var(--slidev-theme-primary, #5d8392);
}

.slidev-keyword--sm {
  font-size: 0.85em;
}

.slidev-keyword--lg {
  font-size: 1.15em;
}
</style>
