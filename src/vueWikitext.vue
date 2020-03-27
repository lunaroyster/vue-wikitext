<script>
import wiky from 'wiky';

export default {
  name: 'VueWikitext', // vue component name
  props: {
    source: {
      type: String,
      default: '',
    }
  },
  computed: {
    html() {
      return wiky.toHtml(this.source)
    }
  },
  methods: {
  },
};
</script>

<template>
  <div class="vueWikitext" v-html="html"></div>
</template>

<style scoped>
  .vueWikitext {
  }
  .vueWikitext p {
  }
</style>
