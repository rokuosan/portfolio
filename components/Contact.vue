<template>
  <div class="w-full">
    <div class="py-20 md:w-5/6 w-[95%] mx-auto relative md:border-l-4 border-neutral-600">
      <!--   Vertical Border   -->
      <div class="absolute origin-bottom-left -rotate-90 text-4xl bottom-5 left-0 md:visible invisible italic select-none text-neutral-600">
        Social
      </div>
      <!--  Title    -->
      <div class="w-fit px-8 text-4xl border-b-2 border-indigo-500 text-center rounded mb-3 mx-auto">
        Contact
      </div>
      <!-- Description -->
      <div class="md:w-fit text-lg text-center mb-8 mx-auto font-notosans">
        御用の際はこちらのメールアドレスにお願いします。
      </div>

      <div class="flex flex-wrap gap-8 px-8 justify-items-center justify-center">
        <div class="sm:p-4 p-2 rounded-2xl w-fit hover:bg-neutral-800" @click="goTo('mailto:rokuosan.dev@gmail.com')">
          <div class="flex gap-4 flex-row">
            <div class="bg-indigo-800 sm:rounded-2xl rounded-xl sm:p-4 p-2">
              <EmailIcon :size="24" />
            </div>
            <div class="grow flex items-center">
              <span class="text-lg sm:text-2xl break-words">rokuosan.dev@gmail.com</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import EmailIcon from 'vue-material-design-icons/Email.vue'

export default {
  name: 'Contact',
  data(){
    return {
      size: 24
    }
  },
  components: {
    EmailIcon
  },
  methods: {
    goTo(url){
      window.open(url, '_blank', 'noreferrer')
    },
    compute(){
      this.size =  window.innerWidth > 640 ? 24 : 12
    }
  },
  mounted () {
    window.addEventListener('resize', () => this.compute())
  }
}
</script>

<style scoped>

</style>
