<template>
  <div class="w-full">
    <div class="py-20 md:w-5/6 w-[95%] mx-auto relative md:border-l-4 border-neutral-600">
      <!--   Vertical Border   -->
      <div class="absolute origin-bottom-left -rotate-90 text-4xl bottom-5 left-0 md:visible invisible italic select-none text-neutral-600">
        Social
      </div>
      <!--  Title    -->
      <div class="w-fit px-8 text-4xl border-b-2 border-indigo-500 text-center rounded mb-3 mx-auto">
        Social
      </div>
      <!-- Description -->
      <div class="md:w-fit text-lg text-center mb-8 mx-auto font-notosans">
        雑に運用しているアカウントです。仲良くしてください。
      </div>
      <!--  Cards    -->
      <div class="flex flex-wrap gap-8 px-8 justify-items-center justify-center">
        <div v-for="social in socials" :key="social.name" :class="social.name">
          <div class="p-4 rounded-2xl sm:w-96 w-72 hover:bg-neutral-800" @click="goTo(social.link)">
            <div class="flex gap-4 flex-row">
              <div class="bg-indigo-800 sm:rounded-2xl rounded-xl p-4">
                <component :is="social.icon" :size="32"  />
              </div>
              <div class="grow flex items-center">
                <span class="text-lg sm:text-2xl break-words">{{social.account}}</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import GitHubIcon from '../node_modules/vue-material-design-icons/GitHub.vue'
import TwitterIcon from 'vue-material-design-icons/Twitter.vue'

export default {
  name: 'Social',
  data () {
    return {
      return: {
      }
    }
  },
  components: {
    TwitterIcon,
    GitHubIcon,
  },
  methods: {
    goTo(url){
      window.open(url, '_blank', 'noreferrer')
    }
  },
  computed: {
    socials(){
      return [
        {
          name: 'Twitter',
          account: '@rokuosan_dev',
          link: 'https://twitter.com/rokuosan_dev',
          icon: TwitterIcon
        },
        {
          name: 'GitHub',
          account: 'rokuosan',
          link: 'https://github.com/rokuosan',
          icon: GitHubIcon
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
