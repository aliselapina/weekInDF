<template>
  <div class="friday content">
    <img src="@/assets/friday.png" alt="friday">

    <h1 class="friday-color">{{ message.title[currentLocale] }}</h1>
    <br />
    <p>{{ message.content[currentLocale] }}</p>

    <div class="footer friday-color">
      <select v-model="currentLocale">
          <option
          selected="English"
          v-for="locale in locales"
          v-bind:key="locale.id"
          v-bind:value="locale.id"
          >
            {{locale.name}}
          </option>
      </select>
      <div>Made by Alise</div>
    </div>

  </div>
</template>

<script>
export default {
  data () {
    return {
      message: {
        title: {
          en: 'Title',
          lv: 'Virsraksts'
        },
        content: {
          en: 'Some huge text',
          lv: 'Garš teksts, kas neiederas dizainā'
        }
      },
      currentLocale: 'en',
      locales: [
        { id: 'en', name: 'English' },
        { id: 'lv', name: 'Latviešu' }
      ]
    }
  }
}
</script>
