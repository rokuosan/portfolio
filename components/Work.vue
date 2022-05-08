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
      <div class="md:w-48 text-4xl border-b-2 border-indigo-500 text-center rounded mb-8 mx-auto">
        Works
      </div>
      <!--  Cards    -->
      <div class="grid 2xl:grid-cols-3 lg:grid-cols-2 grid-cols-1 gap-8 px-8 justify-items-center">
        <Card title="Teleport Assist" description="プレイヤーにインタラクティブなテレポート手段を新たに提供するプラグイン。"
              :tags="['Minecraft', 'Plugin']" link="https://github.com/rokuosan/teleport-assist"/>
        <Card title="Paper Downloader" description="Paper MC をバージョン指定してダウンロード可能な簡易インターフェース。"
              :tags="['Minecraft', 'Application']" link="https://github.com/rokuosan/paper-downloader-nuxt2"/>
        <Card title="Inspect Horse" description="馬の速度と跳躍力のパラメータが取得できるコマンドを追加するプラグイン。"
              :tags="['Minecraft', 'Plugin']" link="https://github.com/rokuosan/inspecthorse"/>
        <Card title="The half of One Hundred Poems" description="百人一首の下50首のみを最短で覚えるためのWebアプリケーション"
              :tags="['Application', 'Fun']" link="https://github.com/rokuosan/onehundredpoems"/>
        <Card title="Kotlin Fullstack...? Slide"
              description="Kotlin/JS で躓いてKotlinのフルスタックアプリケーションに失敗した話をLT向けにまとめたスライド。"
              :tags="['Slide', 'Fun']" link="https://speakerdeck.com/rokuosan/kotlinwoshi-tutemaikuraqing-woi"/>
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
  }
}
</script>

<style>
</style>
