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
  <div class="wrapper">

    <appHeader />
    <!-- other content -->
    <appFooter />
  </div>
</template>

<style scoped>
.wrapper {
  margin: 0 7rem;
}
</style>
