<script setup lang="ts">
type QuoteSize = 'sm' | 'md' | 'lg'

// biome-ignore lint/correctness/noUnusedVariables: props are used in template
const props = withDefaults(
  defineProps<{
    author?: string
    size?: QuoteSize
  }>(),
  { size: 'md' }
)
</script>

<template>
  <blockquote class="slidev-quote" :class="[`slidev-quote--${props.size}`]">
    <div class="slidev-quote__text">
      <slot />
    </div>
    <footer v-if="$slots.author || props.author" class="slidev-quote__author">
      <slot name="author">— {{ props.author }}</slot>
    </footer>
  </blockquote>
</template>

<style scoped>
.slidev-quote {
  border-left: 0.25em solid var(--slidev-theme-primary, #5d8392);
  padding: 0.5em 2em;
  margin: 1rem auto;
  font-style: italic;
  width: fit-content;
  line-height: 1.5;
}

.slidev-quote__text {
  opacity: 0.95;
  font-size: 1.25em;
}

.slidev-quote__author {
  margin-top: 0.75rem;
  font-style: normal;
  font-size: 0.9em;
  opacity: 0.85;
  text-align: right;
  font-style: italic;
}

/* size variants — md is the default (current values) */
.slidev-quote--sm {
  font-size: 1rem;
}

.slidev-quote--lg {
  font-size: 1.5rem;
}
</style>
