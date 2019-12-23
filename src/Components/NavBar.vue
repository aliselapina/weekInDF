<template>
  <div id="nav">
    <router-link class="nav-item" id="monday-nav" to="/">{{title.monday[locale]}}</router-link>
    <router-link class="nav-item" id="tuesday-nav" to="/tuesday">{{title.tuesday[locale]}}</router-link>
    <router-link class="nav-item" id="wednesday-nav" to="/wednesday">{{title.wednesday[locale]}} </router-link>
    <router-link class="nav-item" id="thursday-nav" to="/thursday">{{title.thursday[locale]}} </router-link>
    <router-link class="nav-item" id="friday-nav" to="/friday">{{title.friday[locale]}} </router-link>
    <router-link class="nav-item" id="saturday-nav" to="/saturday">{{title.saturday[locale]}} </router-link>
    <router-link class="nav-item" id="sunday-nav" to="/sunday">{{title.sunday[locale]}}</router-link>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    locale: { type: String, required: true }
  },
  data () {
    return {
      title: {
        monday: { en: 'Monday', lv: 'Pirmdiena' },
        tuesday: { en: 'Tuesday', lv: 'Otrdiena' },
        wednesday: { en: 'Wednesday', lv: 'Treðdiena' },
        thursday: { en: 'Thursday', lv: 'Ceturtdiena' },
        friday: { en: 'Friday', lv: 'Piektdiena' },
        saturday: { en: 'Saturday', lv: 'Sestdiena' },
        sunday: { en: 'Sunday', lv: 'Svçtdiena' }
      }
    }
  }
}
</script>

<style lang="scss">
  .nav-item{
    padding: 10px;
  }
</style>
