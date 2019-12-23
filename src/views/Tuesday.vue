<template>
  <div class="friday content">
    <img src="@/assets/tuesday.png" alt="tuesday">

    <h1 class="friday-color">{{ message.title[locale] }}</h1>
    <br />
    <p>{{ message.content[locale] }}</p>

  </div>
</template>

<script>
export default {
  name: 'Tuesday',
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
