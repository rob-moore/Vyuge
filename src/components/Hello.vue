<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <ul>
      <li v-for="essLink in essLinks">
        <a :href="essLink.link" target="_blank">{{ essLink.text }}</a>
      </li>
      <br>
      <li><a href="http://vuejs-templates.github.io/webpack/" target="_blank">Docs for This Template</a></li>
    </ul>
    <h2>Ecosystem</h2>
    <ul>
      <li v-for="ecoLink in ecoLinks">
        <a :href="ecoLink.link" target="_blank">{{ ecoLink.text }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data() {
    return {
      msg: Date(),
      essLinks: [
        { text: 'Core Docs', link: 'https://vuejs.org' },
        { text: 'Forum', link: 'https://forum.vuejs.org' },
        { text: 'Gitter chat', link: 'https://gitter.im/vuejs/vue' },
        { text: 'Twitter', link: 'https://twitter.com/vuejs' },
      ],
      ecoLinks: [
        { text: 'vue-router', link: 'http://router.vuejs.org/' },
        { text: 'vuex', link: 'http://vuex.vuejs.org/' },
        { text: 'vue-loader', link: 'http://vue-loader.vuejs.org/' },
        { text: 'awesome-vue', link: 'https://github.com/vuejs/awesome-vue' },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
