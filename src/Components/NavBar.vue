<template>
  <div id="nav">
    <router-link class="nav-item" to="/">{{title.monday[locale]}}</router-link>
    <router-link class="nav-item" to="/tuesday">{{title.tuesday[locale]}}</router-link>
    <router-link class="nav-item" to="/wednesday">{{title.wednesday[locale]}} </router-link>
    <router-link class="nav-item" to="/thursday">{{title.thursday[locale]}} </router-link>
    <router-link class="nav-item" to="/friday">{{title.friday[locale]}} </router-link>
    <router-link class="nav-item" to="/saturday">{{title.saturday[locale]}} </router-link>
    <router-link class="nav-item" to="/sunday">{{title.sunday[locale]}}</router-link>
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
        wednesday: { en: 'Wednesday', lv: 'Tresdiena' },
        thursday: { en: 'Thursday', lv: 'Ceturtdiena' },
        friday: { en: 'Friday', lv: 'Piektdiena' },
        saturday: { en: 'Saturday', lv: 'Sestdiena' },
        sunday: { en: 'Sunday', lv: 'Svetdiena' }
      }
    }
  }
}
</script>

<style lang="scss">
  .nav-item{
    padding: 10px;
    text-decoration: none;
    color: midnightblue;
  }
</style>
