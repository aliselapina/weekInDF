<template>
  <div class="friday content">
    <div class="page-content">
      <img src="@/assets/sunday.png" alt="sunday">
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
  name: 'Sunday',
  props: {
    locale: { type: String, required: true }
  },
  data () {
    return {
      message: {
        title: { en: 'Seventh Day', lv: 'Septītā diena' },
        content: {
          en: 'Sunday- funday! Maybe not always. Sundays are nice, there is an excuse not to do anything because it is Sunday but you have to start thinking about the upcoming events next week. But Sunday mornings are still very slow for me. Even slower than Saturdays. If a student is lucky and does not have to go to university on a Monday, Sundays are definitely great days. I like to spend the Sunday outdoors, walking with my dog in the woods or along the sea. If I have not slept well, i do it on a Sunday. Sunday is my favorite day of the week. I am not afraid of Mondays, which are approaching so fast, because Mondays are like a new beginnings. Sundays are my days.',
          lv: 'Sunday- funday! Varbūt arī ne vienmēr. Svētdienas ir jaukas, ir attaisnojums neko nedarīt, jo ir taču svētdiena, taču ir jāsāk domāt jau par gaidāmajiem notikumiem nākošajā nedēļā. Bet Svētdienas rīti arī man tomēr ir nesteidzīgi un pavisam lēni. Vēl lēnāki nekā sestdienās. Ja studentam ir palaimējies un pirmdienā nav jāiet uz universitāti, tad svētdienas noteikti ir lieliskas dienas. Man patīk svētdienu pavadīt pie dabas, ar savu suni aizbraukt pastaigā uz mežu vai gar jūru. Ja neesmu izgulējusies, tad arī to var izdarīt svētdienā. Svētdienas laikam ir manas mīļākās dienas nedēļā. Mani nebaida pirmdienas, kas tik strauji tuvojas, jo pirmdienas taču ir kā jauna sākums. Svētdienas ir manas dienas. '
        }
      }
    }
  }
}
</script>
