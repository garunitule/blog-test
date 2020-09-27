<template>
  <div class="container">
    <div>
      <div v-html="$md.render(post)"></div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      post: '# Goの変数宣言\n解説します。\n```go\nvar name = "go"\n```\n![]()\n'
    }
  },
  mounted() {
    Prism.highlightAll()
  },
}
</script>