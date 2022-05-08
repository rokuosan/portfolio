<template>
  <div class="w-full" id="Works">
    <div class="py-20 min-h-screen md:w-5/6 w-[95%] mx-auto relative md:border-l-4 border-neutral-600">
      <!--   Vertical Border   -->
      <div class="absolute origin-bottom-left -rotate-90 text-4xl bottom-5 left-0 md:visible invisible italic select-none text-neutral-600">
        Works
      </div>
      <!--   Arrow   -->
      <div class="absolute bottom-0 w-full flex justify-center">
        <ArrowDownIcon :size="32"/>
      </div>
      <!--  Title    -->
      <div class="md:w-48 text-4xl border-b-2 border-indigo-500 text-center rounded mb-4 mx-auto">
        Works
      </div>
      <!-- Description -->
      <div class="md:w-fit text-lg text-center mb-12 mx-auto font-notosans">
        現在公開している制作物です。
      </div>
      <!--  Cards    -->
      <div class="grid 2xl:grid-cols-3 lg:grid-cols-2 grid-cols-1 gap-8 px-8 justify-items-center">
        <div v-for="work in works" :key="work.title">
          <div class="col-span-1 sm:w-96 w-64 bg-neutral-800 rounded-2xl relative md:hover:drop-shadow-[0_25px_25px_rgba(0,0,0,0.35)]">
            <h4 class="text-3xl p-4 pb-2"> {{ work.title }} </h4>
            <div class="description p-4 pt-2  text-neutral-400 font-mixed"> {{ work.description }} </div>
            <div class="p-4 select-none flex gap-2 flex-wrap w-3/5">
              <div v-for="tag in work.tags" :key="tag.id" class="rounded-3xl bg-neutral-500 w-fit px-3"> {{ tag }} </div>
            </div>
            <a :href="work.link" class="absolute bottom-4 right-4 after:content-['>>']" rel="noreferrer noopener" target="_blank"> See more </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ArrowDownIcon from 'vue-material-design-icons/ChevronDown.vue'

export default {
  name: 'Work',
  components: {
    ArrowDownIcon
  },
  computed: {
    works(){
      return [
        {
          title: 'Teleport Assist',
          tags: ['Minecraft', 'Plugin'],
          link: 'https://github.com/rokuosan/teleport-assist',
          description: 'プレイヤーにインタラクティブなテレポート手段を新たに提供するプラグイン。'
        },
        {
          title: 'Paper Downloader',
          tags: ['Minecraft', 'Application'],
          link: 'https://github.com/rokuosan/paper-downloader-nuxt2',
          description: 'Paper MC をバージョン指定してダウンロード可能な簡易インターフェース。'
        },
        {
          title: 'Inspect Horse',
          tags: ['Minecraft', 'Plugin'],
          link: 'https://github.com/rokuosan/inspecthorse',
          description: '馬の速度と跳躍力のパラメータが取得できるコマンドを追加するプラグイン。'
        },
        {
          title: 'The half of One Hundred Poems',
          tags: ['Application', 'Fun'],
          link: 'https://github.com/rokuosan/onehundredpoems',
          description: '百人一首の下50首のみを最短で覚えるためのWebアプリケーション'
        },
        {
          title: 'Kotlin Fullstack...? Slide',
          tags: ['Slide', 'Fun'],
          link: 'https://speakerdeck.com/rokuosan/kotlinwoshi-tutemaikuraqing-woi',
          description: 'Kotlin/JS で躓いてKotlinのフルスタックアプリケーションに失敗した話をLT向けにまとめたスライド。'
        }
      ]
    }
  }
}
</script>

<style>
</style>
