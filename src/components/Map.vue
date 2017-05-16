<template lang="jade">
div style="height: 100%"
  p {{ greeting }} World!
  v-map :zoom=13 :center="[47.413220, -1.219482]"
    v-tilelayer url="http://{s}.tile.osm.org/{z}/{x}/{y}.png"
    v-marker :lat-lng="[47.413220, -1.219482]"
</template>

<script>
import Vue2Leaflet from 'vue2-leaflet';

const Map = {
  data() {
    return {
      greeting: 'Hello'
    }
  },
  components: {
    'v-map': Vue2Leaflet.Map,
    'v-tilelayer': Vue2Leaflet.TileLayer,
    'v-marker': Vue2Leaflet.Marker
  }
};

export default Map;
</script>

<style lang="stylus">
@import "~leaflet/dist/leaflet.css";

p
  font-size 2em
  text-align center
</style>
