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
  <!-- other content -->
  <appFooter />
</template>

<style scoped>
.wrapper {
  margin: 0 7rem;
}
</style>
