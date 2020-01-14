<template>
  <div class="friday content">
    <div class="page-content">
      <img src="@/assets/tuesday.png" alt="tuesday">
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
  name: 'Tuesday',
  props: {
    locale: { type: String, required: true }
  },
  data () {
    return {
      message: {
        title: { en: 'Second Day', lv: 'Otrā diena' },
        content: {
          en: 'On tuesday is the traditional annual Chess Tournament of the Faculty of Computer Science. Anyone interested, whether students or lecturers from the University of Latvia, students from other universities or any other fan of this board game, is invited to participate. The tournament is official and its results are always reflected in the personal rankings of the participants. The main prize is the traveling cup of the Faculty of Computer Science - the first bit from the first computer in Latvia. The Student Council usually provides snacks and drinks to participants of the chess tournament. In my opinion, chess is very good game. The best players in it think of algorithms, steps forward, and a way to better solve a problem. And chess is also a good game to play on Tuesday night. The beginning of the week and the two hardest days are over, somehow wanting to calm the mind, but not completely relax - so calm the mind with a slow, thoughtful game of chess. I also like to play chess myself, which my parents taught me in my childhood, but I have played too little, so I am not good at playing tournaments - I know the rules of the game, but I do not know any strategies or relationships between opponent moves. Watching chess though is not very interesting. Especially professional chess. The moves are slow and it is difficult to see the strategies of the players, the thoughts in the head, which hinder concentration and the desire to rush players. At least for me it is. But maybe if I could teach myself to play chess better, then I might also enjoy watching other people play it.',
          lv: 'Otrdienā notiek tradicionālais ikgadējais atklātais Datorikas fakultātes Šaha turnīrs. Tajā ir aicināts piedalīties jebkurš interesents, gan Latvijas Universitātes studenti un pasniedzēji, gan citu augstskolu studenti, gan arī jebkurš cits šīs galda spēles cienītājs. Turnīrs ir oficiāls, tā rezultāti vienmēr tiek atspoguļoti dalībnieku personīgajos reitingos. Galvenā balva ir Datorikas fakultātes ceļojošais kauss – pirmais bits no pirmā Latvijas datora. Blakus telpā parasti Studentu pašpārvalde sagādā šaha turnīra dalībniekiem uzkodas un dzērienus. Manuprāt, šahs ļoti piestāv datoriķiem. Labākie spēlētāji tajā domā algoritmus, soļus uz priekšu un veidu kā labāk atrisināt kādu problēmu. Un arī otrdienas vakaram piestāv šahs. Nedēļas sākums, bet divas grūtākās dienas aizvadītas, gribas kaut kā nomierināt prātu, bet pilnībā atslābt vēl nedrīkst – tāpēc jānomierina prāts ar lēnu, domīgu šaha spēli. Man pašai arī patīk spēlēt šahu, to man vecāki iemācīja jau bērnībā, bet esmu maz spēlējusi, tāpēc es nespēlēju tik labi, lai piedalītos turnīros – zinu spēles noteikumus, taču nezinu nevienu stratēģiju vai sakarības starp pretinieka gājieniem. Skatīties šahu gan nav diez ko interesanti. Jau īpaši profesionālo šahu. Gājieni ir lēni un grūti ir pamanīt spēlētāju stratēģijas, galvā šaujas domas, kas traucē koncentrēties un gribas steidzināt spēlētājus. Vismaz man tā ir. Bet varbūt, ja es pati mācētu labāk spēlēt šahu, tad man varbūt arī patiktu skatīties kā citi cilvēki to spēlē. '
        }
      }
    }
  }
}
</script>
