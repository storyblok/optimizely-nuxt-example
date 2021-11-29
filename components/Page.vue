<template>
  <div v-editable="blok" class="px-6">
    <component :is="blok.component" v-for="iblok in blok.body" :key="iblok._uid" :blok="iblok" />
  </div>
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
