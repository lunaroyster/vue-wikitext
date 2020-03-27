<script>
import Vue from 'vue';
import VueWikitext from './vueWikitext.vue';

export default Vue.extend({
  name: 'ServeDev',
  components: {
    'vue-wikitext': VueWikitext
  },
  data() {
    return {
      wikitext: `=Welcome to vue-wikitext=\n\n%vue-wikitext% is a vue.js component that renders wikitext. It makes use of [https://goessner.net/articles/wiky/ Stefan Gössner's Wiky] library under the hood to convert wikitext to HTML.\n\n==== Try it ====\n\nTry this component by editing the wikitext in the box below.`,
    }
  }
});
</script>

<template>
  <div id="app">
    <vue-wikitext class="wikitext" :source="wikitext" />
    <textarea id="wikitextarea" v-model="wikitext" />
  </div>
</template>

<style>
body {
  margin: 0em;
}

::-webkit-scrollbar {
  width: 8px;
  background-color: #ddd; /* or add it to the track */
}
::-webkit-scrollbar-thumb {
  background-color: #aaa;
}


#app {
  display: flex;
  flex-direction: column;
}
.wikitext {
  height: 60vh;
  padding: 1em;
  box-sizing: border-box;
  overflow-x: auto;
  font-family: sans-serif;
}
#wikitextarea {
  width: 100%;
  height: 40vh;
  border: none;
  outline: none;
  background: #eee;
  padding: 2em;
  box-sizing: border-box;
  resize: none;
}
</style>
