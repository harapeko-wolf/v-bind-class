<template>
  <div class="hello">
    <p>
      Hello,
      <span v-bind:class="{large:isSize}">Vue.js</span>
    </p>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  data: () => ({
    isSize: true
  })
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.large {
  font-size: 32px;
}
</style>
