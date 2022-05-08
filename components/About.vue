<template>
  <div class="w-full">
    <div class="py-20 md:w-5/6 w-[95%] mx-auto relative md:border-l-4 border-neutral-600">
      <!--   Vertical Border   -->
      <div class="absolute origin-bottom-left -rotate-90 text-4xl bottom-5 left-0 md:visible invisible italic select-none text-neutral-600">
        About Me
      </div>
      <div class="absolute bottom-0 w-full flex justify-center">
        <ArrowDownIcon :size="32"/>
      </div>

      <!--  Title    -->
      <div class="w-fit px-8 text-4xl border-b-2 border-indigo-500 text-center rounded mb-4 mx-auto">
        About Me
      </div>
      <!-- Description -->
      <div class="w-fit text-4xl mb-24 mx-auto font-notosans p-4 font-bold tracking-wide leading-relaxed">
        <p>
          バックエンドに興味がある情報系の学生です。
        </p>
        <p>
          Kotlin と自宅サーバーで遊んでます。
        </p>
      </div>

    </div>
  </div>
</template>

<script>
import ArrowDownIcon from 'vue-material-design-icons/ChevronDown.vue'

export default {
  name: 'About',
  components: {
    ArrowDownIcon
  }
}
</script>

<style scoped>

</style>
