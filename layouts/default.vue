<!--suppress CssUnusedSymbol -->
<template>
  <div class="relative w-screen">
    <Header />
    <Nuxt />
  </div>
</template>
<script>
import Header from '@/components/Header'

export default {
  components: {
    Header
  }
}
</script>
<style>
.page-enter, .page-leave-to{
  opacity: 0;
}
.page-enter-active, .page-leave-active{
  transition: opacity .4s;
}
.layout-enter, .layout-leave-active{
  opacity: 0;
}
.layout-enter-active, .layout-leave-active{
  transition: opacity .4s;
}
</style>
