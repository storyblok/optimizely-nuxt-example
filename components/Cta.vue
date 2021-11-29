<template>
  <section v-editable="blok" class="text-gray-600 body-font">
    <div class="container px-5 py-24 mx-auto">
      <div class="lg:w-2/3 flex flex-col sm:flex-row sm:items-center items-start mx-auto">
        <h1 class="flex-grow sm:pr-16 text-2xl font-medium title-font text-gray-900">{{ blok.text }}</h1>
        <button
          class="
            flex-shrink-0
            text-white
            bg-purple-500
            border-0
            py-2
            px-8
            focus:outline-none
            hover:bg-purple-600
            rounded
            text-lg
            mt-10
            sm:mt-0
          "
        >
          {{ blok.button_text }}
        </button>
      </div>
    </div>
  </section>
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
