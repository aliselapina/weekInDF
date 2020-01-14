<template>
  <div class="friday content">
    <div class="page-content">
      <img src="@/assets/wednesday.png" alt="wednesday">
    </div>
    <div class="page-content">
      <h1 class="page-content">{{ message.title[locale] }}</h1>
      <br />
      <p>{{ message.content[locale] }}</p> </div>
    </div>
</template>

<script>
export default {
  name: 'Wednesday',
  props: {
    locale: { type: String, required: true }
  },
  data () {
    return {
      message: {
        title: { en: 'Third Day', lv: 'Trešā diena' },
        content: {
          en: 'Day Three - Computer Games Evening and Tournaments. The Student Council of the Faculty of Computer Science hosts Open League of Legends and CS GO tournaments, where students from any university can form their own team and compete for the title of the strongest team. The computer game culture is widespread amongst computer scientists, allowing you to both demonstrate responsiveness and strategic thinking, and spend great time with friends in a positive atmosphere. For these reasons, Wednesday night is spent with friends and computer games. Although I have not yet been involved in this part of the computer culture, during my childhood my parents tried not tie me to playing computer games so I would not waste time, so I get involved in other ways when there are computer game tournaments at university. And it is possible for anyone! First of all, there is an opportunity to organize these tournaments. Announce them, book the auditoriums, make sure everyone has enough space at computers, make sure everyones computer works, get snacks and drinks, prepare prizes, reward teams at tournaments and, after all, just spend time watching your friends play and understand if that does not seem interesting to you.Tournaments usually take place at the end of the day, when all the lectures and works are over to end the day on a pleasant and interesting tone.Often these tournaments run late into the night, and it is also an adventure to play computer games with your friends after midnight at university! Wednesday like this is a good Wednesday.',
          lv: 'Trešā diena – datorspēļu vakars un turnīri. Datorikas fakultātes Studentu pašpārvalde rīko atvērto League of  Legends un CS GO turnīrus, kurā jebkuras augstskolas studenti var veidot savu komandu un cīnīties par spēcīgākās komandas titulu. Datorspēļu kultūra ir plaši izplatīta datoriķu starpā, tā ļauj gan pierādīt reakciju un stratēģisko domāšanu, gan pavadīt lielisku laiku ar draugiem pozitīvā gaisotnē. Šo iemeslu dēļ, trešdienas vakars tiek pavadīts draugu un datorspēļu vidū. Es pati gan neesmu vēl iesaistījusies šajā datoriķu kultūras daļā, bērnībā man vecāki centās nepieradināt pie datorspēlēm, lai netērētu lieki laiku, tāpēc, kad universitātē notiek datorspēļu turnīri, es iesaistos citos veidos. Un tas ir iespējams jebkuram! Pirmkārt jau, ir iespēja organizēt šos turnīrus. Izsludināt, sarunāt telpas, nodrošināt, lai visiem pietiktu vietas pie datoriem, nodrošināt, lai visiem viss strādā, sagādāt uzkodas un dzērienus atpūtas pauzēm, sagatavot balvas, turnīru galā apbalvot komandas un galu galā var arī vienkārši pavadīt laiku, skatoties kā draugiem iet un saprast vai pašam kas tāds nesāk šķist interesants. Turnīri parasti notiek dienas beigās, kad visiem lekcijas un darbi jau beigušies, lai diena noslēgtos ar patīkamo un interesanto. Bieži vien šie turnīri ievelkas līdz pat vēlai naktij, un arī tas ir piedzīvojums – universitātē spēlēt datorspēles ar draugiem pēc pusnakts! Tādas trešdienas ir labas trešdienas. '
        }
      }
    }
  }
}
</script>
