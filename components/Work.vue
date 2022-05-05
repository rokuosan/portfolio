<template>
  <div class="w-full bg-neutral-50">
    <div class="py-20 md:w-5/6 w-[95%] mx-auto relative md:border-l-4 border-neutral-900">
      <!--   Vertical Border   -->
      <div class="absolute origin-bottom-left -rotate-90 text-4xl bottom-5 left-0 md:visible invisible italic select-none text-neutral-900">
        Works
      </div>
      <!--  Cards    -->
      <div class="grid xl:grid-cols-4 lg:grid-cols-3 md:grid-cols-2 grid-cols-1 gap-8 text-neutral-900 px-8">
        <div class="border border-neutral-500 col-span-1">
          <h4 class="text-3xl">Teleport Assist</h4>
          <a href="https://github.com/rokuosan/teleport-assist" target="_blank" ref="noopener noreferrer">View on GitHub</a>
        </div>
        <div class="border border-neutral-500 col-span-1">
          <h4 class="text-3xl">Paper Downloader</h4>
          <a href="https://github.com/rokuosan/paper-downloader-nuxt2" target="_blank" ref="noopener noreferrer">View on GitHub</a>
        </div>
        <div class="border border-neutral-500 col-span-1">
          <h4 class="text-3xl">Inspect Horse</h4>
          <a href="https://github.com/rokuosan/inspecthorse" target="_blank" ref="noopener noreferrer">View on GitHub</a>
        </div>
        <div class="border border-neutral-500 col-span-1">
          <h4 class="text-3xl">The half of One Hundred Poems</h4>
          <a href="https://github.com/rokuosan/onehundredpoems" target="_blank" ref="noopener noreferrer">View on GitHub</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Work'
}
</script>

<style>
</style>
