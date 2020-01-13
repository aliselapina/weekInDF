<template>
  <div class="friday content">
    <div class="page-content">
      <img src="@/assets/friday.png" alt="friday">
      </div>
    <div class="page-content">
        <h1 class="page-content">{{ message.title[locale] }}</h1>
        <br />
        <p>{{ message.content[locale] }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Friday',
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
