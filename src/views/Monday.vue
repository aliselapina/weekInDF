<template>
  <div class="friday content">
    <img src="@/assets/monday.png" alt="monday">

    <h1 class="friday-color">{{ message.title[locale] }}</h1>
    <br />
    <p>{{ message.content[locale] }}</p>

  </div>
</template>

<script>
export default {
  name: 'Monday',
  props: {
    locale: { type: String, required: true }
  },
  data () {
    return {
      message: {
        title: { en: 'First Day', lv: 'Pirmā diena' },
        content: {
          en: 'Some huge text',
          lv: 'Viena no iemīļotākajām fakultātes dzimšanas dienas tradīcijām ir lielās dzimšanas dienas kūkas ēšana LU vestibilā, kur uz gabaliņu kūkas sanāk gan fakultātes studenti un mācībspēki, gan LU darbinieki un fakultātes draugi. Pirms tortes griešanas tradicionāli ciemiņus uzrunā Datorikas fakultātes dekāns, WeAreDots vadītājs un Studentu pašpārvaldes priekšsēdētāja.' }
      }
    }
  }
}
</script>
