<template>
  <div class="friday content">
    <div class="page-content">
      <img src="@/assets/saturday.png" alt="saturday">
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
  name: 'Saturday',
  props: {
    locale: { type: String, required: true }
  },
  data () {
    return {
      message: {
        title: { en: 'Sixth Day', lv: 'Sestā diena' },
        content: {
          en: 'It is a holiday. Saturday.Everyone gets up in their own time, depending on what time they have come home from the Jubilee Ball.Thinking about feelings about the experience throughout the week.For the Student Council this Saturday is not as calm and slow as they would like.First of all, it is important to help clean up the ballroom, because usually on Saturday there are various events or lectures at the university.After the ballroom is cleared, they need to start looking back and analyzing the past week.What was good, what was successful, what was bad, what was wrong, what we want to improve next year.It could even be said that the planning for next years celebrations begins the day after the current years celebrations.Later, feedback from visitors is also collected in order to know the impartial opinion of all people.But those who are lucky and do not have to work with the Student Council on Saturday can lazy rest at home, sleep, and start thinking very, very slowly about next week.No one will catch up on homeworks yet, but you may be able to do a weeks delay - read a book, meet friends or spend some leisure time doing some active stuff.Saturdays are my favorite days to make a slow and fullfilling breakfast, have a leisurely coffee and watch the latest series for my favorite TV series.In my opinion, it is just one word that best describes my Saturday - leisurely.',
          lv: 'Ir pienākusi brīvdiena. Sestdiena. Katrs ceļas savā laikā, atkarībā no tā cikos pārradies no Jubilejas balles mājās. Raisās domas par piedzīvoto visas nedēļas garumā. Studentu pašpārvaldei šī sestdiena nav tik mierīga un lēna kā gribētos. Pirmkārt, ir jāpalīdz savākt un sakārtot balles telpas, jo parasti arī sestdienā universitātē notiek dažādi pasākumi vai lekcijas. Pēc balles telpu novākšanas ir jāsāk atskatīties un pagājušo nedēļu un jāizanalizē tā. Kas bija labi, kas izdevās, kas bija slikti, kas neizdevās, ko gribam uzlabot nākamajā gadā. Varētu pat teikt, ka nākamā gada svinības plānot sāk tiktas nākamajā dienā jau pēc aktuālā gada svinībām. Vēlāk tiek ievāktas arī atsauksmes no apmeklētājiem, lai zinātu visu cilvēku objektīvo viedokli. Bet tiem, kuriem palaimējies un sestdienā nav jānodarbojas ar Studentu pašpārvaldes darbiem, var droši mierīgi slinkot un atpūsties pa mājām, izgulēties un ļoti, ļoti lēnām sākt domāt, kas paredzēts nākamajā nedēļā. Mājasdarbiem klāt vēl neviens neķersies, taču var paspēt izdarīt pa nedēļu iekavēto – palasīt kādu grāmatu, satikties ar draugiem vai pavadīt brīvo laiku ar kādu aktīvo atpūtas veidu. Sestdienas ir manas mīļākās dienas, lai uztaisītu lēnas un pilnvērtīgas brokastis, nesteidzīgi izdzert kafiju un noskatīties jaunāku sēriju savam mīļākajam seriālam. Manuprāt tieši viens vārds vislabāk raksturo manas sestdienas  - nesteidzīgi. '
        }
      }
    }
  }
}
</script>
