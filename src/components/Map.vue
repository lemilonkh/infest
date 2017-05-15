<template>
  <v-map :zoom=13 :center="[47.413220, -1.219482]">
    <v-tilelayer url="http://{s}.tile.osm.org/{z}/{x}/{y}.png"></v-tilelayer>
    <v-marker :lat-lng="[47.413220, -1.219482]"></v-marker>
  </v-map>
</template>

<script>

</script>

<style lang="stylus">
  @import "~leaflet/dist/leaflet.css";
</style>
