<template>
  <div class="friday content">
<<<<<<< HEAD
    <div class="page-content">
      <img  src="@/assets/monday.png" alt="monday">
    </div>
    <div class="page-content">
      <h1 >{{ message.title[locale] }}</h1>
      <br />
      <p>{{ message.content[locale] }}</p>
    </div>
=======
    <h1 class="friday-color">{{ message.title[locale] }}</h1>
    <br />
    <p>{{ message.content[locale] }}</p>

>>>>>>> 618cfe1662791f7bf3ab6f372284153379deb4cc
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
