<template>
  <div class="friday content">
    <div class="page-content">
      <img  src="@/assets/monday.png" alt="monday">
    </div>
    <div class="page-content">
      <h1 >{{ message.title[locale] }}</h1>
      <br />
      <p>{{ message.content[locale] }}</p>
    </div>
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
          en: 'One of the favorite birthday traditions of the faculty is eating the big birthday cake in the lobby of the University of Latvia, where students and faculty staff and friends gather for a piece of cake. It also often starts the Computer Week birthday week (though it depends on the days of the week and the date, since DFs birthday is on March 16, and the cake is eaten either on the 16th, or if it falls in weekend, then Monday or Friday, respectively).Before the cake is cut, the guests are traditionally addressed by Guntis Arnicans, Dean of the Faculty of Computer Science, and one of the supporters of the Faculty of Computer Science(Squalio, ScandiWeb, Accenture or someone else) who has sponsored the birthday cake and prepared a gift for the Faculty, Chairman of the Student Council, this year that is Artis Ivo Pencis.Cake eating usually involves cheerful conversations, a chance to meet masters or PhD students who are not daily on Rainis Boulevard 19 and talk to them to learn something new.On the first day of the week of the facultys birthday, students have a chance to see birthday decorations prepared by the Student Council and its activists each year. The decorations are usually made in faculty colors that are dark blue and gold. They are usually matched with white, black and gray. The day is usually peaceful and joyful as everyone is cheered up by a piece of cake that gives them motivation to cope with the hardest day of the week - Monday.',
          lv: 'Viena no iemīļotākajām fakultātes dzimšanas dienas tradīcijām ir lielās dzimšanas dienas kūkas ēšana LU vestibilā, kur uz gabaliņu kūkas sanāk gan fakultātes studenti un mācībspēki, gan LU darbinieki un fakultātes draugi. Tā arī bieži iesākas Datorikas Fakultātes dzimšanas dienas nedēļa (tas gan ir atkarīgs no tā, kā iekrīt nedēļas dienas un mēneša datumi, jo DF dzimšanas diena ir 16.martā, un kūkas ēšana notiek vai nu tieši 16.datumā, vai, ja tas iekritis brīvdienā, tad attiecīgi pirmdienā vai piektdienā, kas tuvāk). Pirms tortes griešanas tradicionāli ciemiņus uzrunā Datorikas fakultātes dekāns Guntis Arnicāns, Datorikas Fakultātes kāds no atbalstītājiem (Squalio, ScandiWeb, Accenture vai kāds cits), kuri ir sponsorējuši dzimšanas dienas kūku un arī sagādājuši fakultātei katru gadu kādu dāvanu, un Studentu pašpārvaldes priekšsēdētājs, kas šogad ir Artis Ivo Pencis. Kūkas ēšanas laikā parasti rosās jautras sarunas, ir iespēja satikt maģistrus vai doktorantus, kas ikdienā neuzturas Raiņa bulvārī 19, un aprunāties ar tiem, uzzināt ko jaunu. Pirmajā fakultātes dzimšanas dienas nedēļas dienā arī studentu acīm paveras dzimšanas dienas dekorācijas, ko katru gadu sagatavo Studentu pašpārvalde un tās aktīvisti.Dekorācijas parasti ir taisītas fakultātes krāsās, kas ir tumši zila un zelta.Tām parasti tiek pieskaņoti baltie, melnie un pelēkie toņi. Diena parasti ir mierīga un priecīga, jo visi uzmundrināti ar kūkas gabalu, kas dod motivāciju tik galā ar nedēļas grūtāko dienu – pirmdienu.'
        }
      }
    }
  }
}
</script>
