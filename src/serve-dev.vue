<script>
import Vue from 'vue';
import VueWikitext from '@/vueWikitext.vue';

export default Vue.extend({
  name: 'ServeDev',
  components: {
    VueWikitext
  }
});
</script>

<template>
  <div id="app">
    <vueWikitext />
  </div>
</template>
