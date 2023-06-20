<template>
   <AppMenu />
</template>

<script>
import AppMenu from './components/AppMenu.vue';

export default {
  name: 'App',
  data() {
    return {

    }
  },

  components: {
    AppMenu,
  }
}

</script>

<style lang="scss">
 @import 'bootstrap/scss/bootstrap';
@import "./styles/general.scss";
</style>