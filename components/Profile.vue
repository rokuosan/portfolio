<template>
  <div class="w-full">
    <div class="py-20 grid grid-cols-1 md:grid-cols-3 md:gap-8 gap-y-8 md:w-5/6 w-[95%] mx-auto relative md:border-l-4 border-neutral-700">
      <div class="absolute origin-bottom-left -rotate-90 text-4xl bottom-5 left-0 md:visible invisible italic select-none text-neutral-700">
        Self Introduction
      </div>
      <div class="col-span-1 md:justify-self-end justify-self-center flex relative select-none">
        <img alt="Avatar" src="https://avatars.githubusercontent.com/u/85651386?v=4" class="self-center rounded-full border-8 border-neutral-700 lg:w-64 lg:h-64 w-48 h-48">
      </div>
      <div class="col-span-2">
        <h3 class="text-4xl border-b-2 border-indigo-500">
          Profile
        </h3>
        <div class="grid grid-cols-3 text-2xl pt-5 gap-x-6">
          <div class="col-span-1 key grid grid-cols-1 gap-y-4 text-center font-light">
            <div> Name </div>
            <div> Birthday </div>
            <div> Country </div>
            <div> Favorite </div>
          </div>
          <div class="col-span-2 value grid grid-cols-1 gap-y-4 md:text-left text-center">
            <div> rokuosan </div>
            <div> 03/03 </div>
            <div> Japan </div>
            <div> Kotlin </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Profile'
}
</script>

<style scoped>
body{
  background: rgb(224, 231, 255);
}
</style>
