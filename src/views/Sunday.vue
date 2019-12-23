<template>
  <div class="friday content">
    <img src="@/assets/sunday.png" alt="sunday">

    <h1 class="friday-color">{{ message.title[locale] }}</h1>
    <br />
    <p>{{ message.content[locale] }}</p>

  </div>
</template>

<script>
export default {
  name: 'Sunday',
  props: {
    locale: { type: String, required: true }
  },
  data () {
    return {
      message: {
        title: { en: 'Title', lv: 'Virsraksts' },
        content: { en: 'Some huge text', lv: 'Garš teksts, kas neiederas dizainā' }
      }
    }
  }
}
</script>
