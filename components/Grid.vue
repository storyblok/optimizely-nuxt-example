<template>
  <ul v-editable="blok" class="flex py-8 mb-6">
    <li v-for="iblok in blok.columns" :key="iblok._uid" class="flex-auto px-6">
      <component :is="iblok.component" :blok="iblok" />
    </li>
  </ul>
</template>

<script>
export default {
  props: {
    blok: {
      type: Object,
      required: true,
    },
  },
}
</script>
