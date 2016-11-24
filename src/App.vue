<template lang="pug">
#app.container
  h1 Raider, music for people with bad taste
  h2 Download my crappy music
  ul
    template(v-for="song in songs")
      li
        a(v-bind:href='"mp3/" + song.filename' target='_blank') {{ song.title }}
  pre Right click -> save link as...
  h2 Follow me on the internet
  ul
    li
      a(href='http://twitter.com/ixraider/' target='_blank') Twitter
    li
      a(href='http://soundcloud.com/raider/' target='_blank') Soundcloud
    li
      a(href='http://youtube.com/ixraider' target='_blank') Youtube
    li
      a(href='http://instagram.com/ixraider' target='_blank') Instagram
    li
      a(href='http://facebook.com/officialraider' target='_blank') Faceboob
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Raider',
      songs: [
        { title: "Rain (Raider Remix)", filename: "Astronaut - Rain (Raider Remix).mp3" },
        { title: "Etho's Anthem VIP", filename: "Raider - Etho's Anthem VIP.mp3" },
        { title: "Etho's Anthem", filename: "Raider - Etho's Anthem.mp3" },
        { title: "Futuro", filename: "Raider - Futuro.mp3" },
        { title: "Globe", filename: "Raider - Globe.mp3" },
        { title: "Kaizen", filename: "Raider - Kaizen (Original Mix).mp3" },
        { title: "Ordinance", filename: "Raider - Ordinance (Original Mix).mp3" },
        { title: "Revolution (Remastered)", filename: "Raider - Revolution (Remastered).mp3" },
        { title: "Somnium", filename: "Raider - Somnium.mp3" },
        { title: "The Girl (Raider Remix)", filename: "Raider - The Girl - 01 Hellberg's The Girl feat. Cozi Zuehlsdorff (Raider Remix).mp3" },
        { title: "Tremble (feat. Yoe Mase)", filename: "Raider - Tremble - 01 Tremble (feat. Yoe Mase).mp3" },
        { title: "Vanguard", filename: "Raider - Vanguard.mp3" },
        { title: "Finestorm", filename: "Raider & Lower Sixth - Finestorm.mp3" },
        { title: "Illusion", filename: "Raider & Lower Sixth - Illusion.mp3" },
        { title: "Colors (Raider Remix)", filename: "Tritonal & Paris Blohm - Colors (Raider Remix).mp3" },
      ]
    }
  }
}
</script>

<style lang="sass?indentedSyntax=true">
#app
  font-family: 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  color: #2c3e50
  margin-top: 70px

.container
  max-width: 780px
  margin: 0 auto

h1, h2
  font-weight: normal

ul
  list-style-type: none
  padding: 0

li
  display: inline-block
  margin: 0 10px

a
  color: #42b983
</style>
