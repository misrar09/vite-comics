<script>
import appHeader from './components/appHeader.vue';
import appFooter from './components/appFooter.vue';

export default {
  components: {
    appHeader,
    appFooter,
  }
}

</script>

<template>
  <appHeader />
  <div class="other_cont">

  </div>
  <!-- other content -->
  <appFooter />
</template>

<style scoped>
.wrapper {
  margin: 0 7rem;
}

.other_cont {
  min-width: 100vw;
  min-height: 40rem;
  overflow: auto;
}
</style>
