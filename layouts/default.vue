<!--suppress CssUnusedSymbol -->
<template>
  <div class="relative">
    <Nuxt />
    <Footer />
  </div>
</template>
<script>
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
