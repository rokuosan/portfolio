<template>
  <div class="col-span-1 sm:w-96 w-64 bg-neutral-800 rounded-2xl relative md:hover:drop-shadow-[0_25px_25px_rgba(0,0,0,0.35)]">
    <!-- Card title -->
    <h4 class="text-3xl p-4 pb-2">
      {{ title }}
    </h4>
    <!-- Description -->
    <div class="description p-4 pt-2  text-neutral-400 font-mixed">
      {{ description }}
    </div>

    <!-- Tag -->
    <div class="p-4 select-none flex gap-2 flex-wrap w-3/5">
      <div v-for="tag in tags" :key="tag.id" class="rounded-3xl bg-neutral-500 w-fit px-3">
        {{ tag }}
      </div>
    </div>

    <!-- See more -->
    <a :href="link" class="absolute bottom-4 right-4 after:content-['>>']" rel="noreferrer noopener" target="_blank">
      See more
    </a>
  </div>
</template>
<script>
export default {
  name: 'Card',
  props: {
    title: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    },
    tags: {
      type: Array,
      required: false,
      default: () => ['']
    },
    link: {
      type: String,
      required: true
    }
  }
}
</script>
