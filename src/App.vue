<template>
  <div id="app">
    <NavBar :locale="currentLocale"></NavBar>
    <h1> {{ title[currentLocale]}}</h1>
    <select v-model="currentLocale">
      <option selected="English"
              v-for="locale in locales"
              v-bind:key="locale.id"
              v-bind:value="locale.id">
        {{locale.name}}
      </option>
    </select>
    <router-view :locale="currentLocale"></router-view>

    <div class="footer friday-color">
      <div>{{footer[currentLocale]}} Alise Rasa Lapiņa</div>
    </div>

  </div>
</template>

<script>
import NavBar from '@/Components/NavBar.vue'
export default {
  components: {
    NavBar
  },
  data () {
    return {
      title: { en: 'Birthday week in Faculty of Computing', lv: 'Datorikas fakultātes dzimšanas dienas nedēļa' },
      footer: { en: 'Made by', lv: 'Darba autors:' },
      currentLocale: 'lv',
      locales: [
        { id: 'en', name: 'English' },
        { id: 'lv', name: 'Latviešu' }
      ]
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
