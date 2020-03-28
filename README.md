# Vue Wikitext

A vue component that renders wikitext.

[![Run on Repl.it](https://repl.it/badge/github/lunaroyster/vue-wikitext)](https://repl.it/github/lunaroyster/vue-wikitext)
[![GitHub issues](https://img.shields.io/github/issues/lunaroyster/vue-wikitext)](https://github.com/lunaroyster/vue-wikitext/issues)

## Usage

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
