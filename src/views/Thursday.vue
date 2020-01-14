<template>
  <div class="friday content">
    <div class="page-content">
      <img src="@/assets/thursday.png" alt="thursday">
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
  name: 'Thursday',
  props: {
    locale: { type: String, required: true }
  },
  data () {
    return {
      message: {
        title: { en: 'Fourth Day', lv: 'Ceturtā diena' },
        content: {
          en: 'On the fourth day, there are an evening of board games, inviting students of the Faculty of Computer Science and other faculties to play exciting board games in a friendly atmosphere. Even though board game nights are held about every two months, these events are always very well attended and nobody gets tired of them. Usually board games are displayed in two auditoriums and then the people who come can choose which games they are interested in, collect teams and play from a large selection. In parallel, Just Dance is played in the Classroom. Movements appear on the screen and people have to imitate them as accurately as possible. The one with the most accuracy gets the most points in the game. Recently, supporters of the Faculty of Computing have donated a novus table, and last year Student Council bought table tennis, so since then, novus and table tennis have been played on board game evenings. So there are things for all tastes, from those who like to think hard in complex and long board games, those who like fast and fun board games, and those who want something more active and moving. I myself have tried all these activities, and I am probably a fan of fast and fun board games. My favorites are Hali Gali and Ligretto. Both must have a quick reaction and rapid movements. Board games evenings are my favorite activities at university.',
          lv: 'Ceturtajā dienā notiks galda spēļu vakars, uz kuru aicināti gan Datorikas fakultātes, gan citu fakultāšu studenti, lai draudzīgā gaisotnē spēlētu kādu no aizraujošajām galda spēlēm. Lai gan galda spēļu vakari notiek apmēram reizi divos mēnešos, šie pasākumi vienmēr ir ļoti labi apmeklēti un nevienam neapnīk. Parasti galda spēles tiek izliktas divās auditorijās un tad atnākušie cilvēki var izvēlēties kādas spēles viņiem labāk interesē, vākt komandas un spēlēt spēles no liela sortimenta. Paralēli Mācību telpā notiek arī Just Dance spēlēšana. UZ ekrāna tiek rādītas kustības un cilvēkiem ir maksimāli precīzi tās jāatdarina. Tas, kuram sanācis visprecīzāk, iegūst visvairāk spēles punktus. Nesen Datorikas Fakultātes atbalstītāji uzdāvināja novusa galdu, un pagājušo gad Studentu Pašpārvalde nopirka galda tenisu, tāpēc kopš tā laika galda spēļu vakaros tiek spēlēts arī novuss un galda teniss. Līdz ar to ir atrodamas lietas visām gaumēs – gan tiem, kam patīk vairāk prātot sarežģītās un ilgās galda spēlēs, gan tiem, kam patīk ātrās un jautrās galda spēles, gan arī tiem, kam gribas nedaudz kaut ko aktīvāku un izkustēties. Es pati esmu izmēģinājusi visas šīs aktivitātes, un es laikam esmu ātro un jautro galda spēļu fans. Manas mīļākās ir Hali Gali un Ligretto. Abās ir jābūt ātrai reakcijai un straujām kustībām. Galda spēļu vakari ir manis visiecienītākie pasākumi universitātē. '
        }
      }
    }
  }
}
</script>
