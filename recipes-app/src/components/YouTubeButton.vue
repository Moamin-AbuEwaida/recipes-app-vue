<template>
  <div>
    <a
      :href="href"
      target="_blank"
      class="px-3 py-2 rounded border-2 text-white border-red-600 bg-red-500 hover:bg-white hover:text-red-500 transition-colors"
    >
      <slot></slot>
    </a>
  </div>
</template>

<script setup>
const props = defineProps({
  href: String,
});
</script>

<style></style>
