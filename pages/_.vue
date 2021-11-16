<template>
  <component
    :is="story.content.component"
    v-if="story.content.component"
    :key="story.content._uid"
    :blok="story.content"
  />
</template>

<script>
export default {
  name: 'AbTestPage',
  asyncData(context) {
    const version = context.query._storyblok || context.isDev ? 'draft' : 'published'
    const fullSlug = context.route.path === '/' || context.route.path === '' ? 'home' : context.route.path
    return context.app.$storyapi
      .get(`cdn/stories/${fullSlug}`, {
        version,
      })
      .then((res) => {
        return res.data
      })
  },
  data() {
    return {
      story: { content: {} },
    }
  },
  mounted() {
    this.$storybridge(() => {
      // eslint-disable-next-line no-undef
      const storyblokInstance = new StoryblokBridge()
      // Use the input event for instant update of content
      storyblokInstance.on('input', (event) => {
        if (event.story.id === this.story.id) {
          this.story.content = event.story.content
        }
      })
      // Use the bridge to listen the events
      storyblokInstance.on(['published', 'change'], (event) => {
        this.$nuxt.$router.go({
          path: this.$nuxt.$router.currentRoute,
          force: true,
        })
      })
    })
  },
}
</script>
