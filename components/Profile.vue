<template>
  <div class="py-20 grid grid-cols-1 md:grid-cols-3 md:gap-8 gap-y-8 md:w-5/6 w-[95%] mx-auto font-poppins">
    <div class="col-span-1 md:justify-self-end justify-self-center flex relative select-none">
      <img width="256" height="256" alt="Avatar" src="https://avatars.githubusercontent.com/u/85651386?v=4" class="rounded-full border-4 border-sky-900">
    </div>
    <div class="col-span-2">
      <h3 class="text-4xl border-sky-900 border-b-2">
        Profile
      </h3>
      <div class="grid grid-cols-3 text-2xl pt-5 gap-x-6">
        <div class="col-span-1 key grid grid-cols-1 gap-y-4 text-center font-light">
          <div>
            Name
          </div>
          <div>
            Birthday
          </div>
          <div>
            Country
          </div>
          <div>
            Favorite
          </div>
        </div>
        <div class="col-span-2 value grid grid-cols-1 gap-y-4 md:text-left text-center">
          <div>
            rokuosan
          </div>
          <div>
            03/03
          </div>
          <div>
            Japan
          </div>
          <div>
            Kotlin
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
