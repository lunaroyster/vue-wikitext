## Vue Wikitext 
[![Run on Repl.it](https://repl.it/badge/github/lunaroyster/vue-wikitext)](https://repl.it/github/lunaroyster/vue-wikitext)

A vue component that renders wikitext.

### Usage

```vue
<template>
  <div>
    <vue-wikitext :source="wikitext" />
  </div>
</template>

<script>
export default {
  components: {
    'vue-wikitext': VueWikitext
  },
  data() {
    return {
      wikitext: '=Welcome to vue-wikitext='
    };
  },
}
</script>
```
