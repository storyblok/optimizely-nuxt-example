<template>
  <div v-if="visible" v-editable="blok" class="px-6">
    <component :is="iblok.component" v-for="iblok in blok.body" :key="iblok._uid" :blok="iblok" />
  </div>
</template>

<script>
import { createInstance } from '@optimizely/optimizely-sdk'

export default {
  props: {
    blok: {
      type: Object,
      required: true,
    },
  },
  data() {
    return {
      activatedVariation: null,
    }
  },
  async fetch() {
    const optimizelyClientInstance = createInstance({
      sdkKey: this.$config.optimizelySdkKey,
    })
    await optimizelyClientInstance.onReady()
    this.activatedVariation = optimizelyClientInstance.activate(this.blok.segment.experiment, `user1`)
  },
  computed: {
    visible() {
      return this.blok.segment.variation === this.activatedVariation
    },
  },
}
</script>
