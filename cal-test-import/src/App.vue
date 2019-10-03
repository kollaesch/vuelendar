<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <v-range-selector :start-date.sync="range.start" :end-date.sync="range.end"  />
    <v-day-selector v-model="date"/>
    <v-cal-month class="hero1" v-model="date"/> -->
    <v-cal class="hero1" v-model="date"/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import VRangeSelector from 'vuelendar/components/vl-range-selector';
import VDaySelector from 'vuelendar/components/vl-day-selector';
import VCalMonth from 'vuelendar/components/vl-calendar-month';
import VCal from 'vuelendar/components/vl-calendar';


export default {
  name: 'app',
  components: {
    // HelloWorld,
    // VRangeSelector,
    // VDaySelector,
    // VCalMonth,
    VCal
  },
  data () {
    return {
      range: {},
      date: null
    }
  }
}

</script>

<style src="vuelendar/scss/vuelendar.scss" lang="scss"></style>
<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.km-closed {
  background-color: #c5baba;
  border: 1px;
  border-radius: 20px;
  margin: 2px;
}
.km-open-halfday {
  background-color: yellow;
  border: 1px;
  border-radius: 20px;
  margin: 2px;
}
.km-open-fullday {
  background-color: green;
  border: 1px;
  border-radius: 20px;
  margin: 2px;
}

</style>
