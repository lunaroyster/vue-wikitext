<script>
import Vue from 'vue';
import VueWikitext from '@/vueWikitext.vue';

export default Vue.extend({
  name: 'ServeDev',
  components: {
    'vue-wikitext': VueWikitext
  },
  data() {
    return {
      wikitext: `==Welcome to vue-wikitext==
      Here's an example showing %vue-wikitext% in action.`
    }
  }
});
</script>

<template>
  <div id="app">
    <vue-wikitext :source="wikitext" />
  </div>
</template>
