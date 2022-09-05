<template>
  <div id="app">
    <EventsCalendar></EventsCalendar>
  </div>
</template>

<script>
import EventsCalendar from './components/EventsCalendar.vue';

export default {
  name: 'App',
  components: {
    EventsCalendar
  }
}
</script>

<style lang="scss">
@import './assets/scss/style';
#app {
  padding: 35px 0;
  overflow: hidden;
}
</style>
