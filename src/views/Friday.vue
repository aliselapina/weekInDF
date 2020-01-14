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
        title: { en: 'Fifth Day', lv: 'Piektā diena' },
        content: {
          en: 'Is not that the end of the week? Many peoples favorite and most awaited day - Friday.The biggest event of the week and the culmination of a birthday - a Jubilee celebration at the UL main building with students, teachers, alumni, collaborators and other faculty friends.There will be live music and a ballroom, a history room, a technology room and a photo - shoot - corner during the celebration.This is an event where everyone can come together, celebrate the faculty anniversary and have a nice rest.The annual Computer Awards will also be presented during the event.The Computer Awards of the Year is presented for various nominations - Student of the Year, Teacher of the Year, Employee of the Year, and others like it.The anniversary ball should be prepared for the longest time as it is the biggest birthday week event with the most visitors.The event needs to have multiple bands and musicians, the event needs an evening host, many sponsors are found, and special decorations are made.The birthday party must be special.There is always a photo - shoot - corner where the photographer captures human companies, but the rest of the ball is photographed by another photographer who captures the most beautiful and interesting moments of the ball.So far, I have only participated in organizing these parties, have not attended, but I have only heard good feedback from everyone, including people from other universities.The ball usually starts around ten in the evening and the strongest dancers lasts until five in the morning.Then you can go home safely and the weekend has started successfully!',
          lv: 'Vai tik tās nav nedēļas beigas? Daudzu cilvēku mīļākā un gaidītākā diena ir klāt – Piektdiena. Nedēļas lielākais pasākums un dzimšanas dienas kulminācija - Jubilejas svinības LU galvenajā ēkā kopā ar studējošajiem, pasniedzējiem, absolventiem, sadarbības partneriem un citiem fakultātes draugiem. Svinību laikā būs gan dzīvā mūzika un deju zāle, gan vēstures telpa, gan tehnoloģiju telpa un fotostūris. Šis ir tas pasākums, kur visiem kopā sanākt, nosvinēt fakultātes jubileju un jauki atpūsties. Pasākuma laikā tiks pasniegta arī Datoriķu gada balva. Datoriķu Gada Balvu pasniedz par dažādām nominācijām – gada students, gada pasniedzējs, gada darbinieks, un citām tam līdzīgām. Jubilejas ballei jāgatavojas visilgāk, jo tas ir vislielākais dzimšanas dienas nedēļas pasākums ar visvairāk apmeklētājiem. Pasākumam jāsarunā vairākas grupas un mūziķi, pasākumam tiek sarunāts vakara vadītājs, tiek atrasti daudzi sponsori, tiek veidotas īpašas dekorācijas. Dzimšanas dienas ballei taču jābūt īpašai. Vienmēr pie dekorācijām klāt skaitās arī fotostūrītis, kurā fotogrāfs iemūžina cilvēku kompānijas, bet pārējo balli fotogrāfē otrs fotogrāfs, kas iemūžina skaistākos un interesantākos balles mirkļus. Pati pagaidām esmu piedalījusies tikai šo baļļu organizēšanā, nav sanācis ierasties, bet esmu dzirdējusi tikai labas atsauksmes no visiem, arī no citu universitāšu pārstāvjiem. Balle parasti sākas ap desmitiem vakarā un stiprākie iztur līdz pieciem no rīta. Tad var mierīgi doties mājās un nedēļas nogale ir sākusies veiksmīgi. '
        }
      }
    }
  }
}
</script>
