<template>
  <q-page class="container q-pa-md">
    <div class="row q-px-lg q-pb-sm">
      <div class="col">
        <span class="text-caption">
        Nossa comunidade surgiu juntamente com a popularização do framework Vue.js.<br>
        Tivemos a iniciativa de reunir desenvolvedores e interessados no framework uma vez ao mês,
        para apresentar experiências, técnicas, boas práticas, cases e claro fazer um bom network entre
        a comunidade da nossa região.
        </span>
      </div>
    </div>
    <div class="row">
      <div class="col-12 q-pa-md">
        <q-carousel
          animated
          v-model="slide"
          arrows
          navigation
          infinite
          height="38rem"
        >
          <q-carousel-slide :name="1" img-src="statics/meetup1.JPG" />
          <q-carousel-slide :name="2" img-src="statics/meetup6.jpeg" />
          <q-carousel-slide :name="3" img-src="statics/meetup3.jpeg" />
          <q-carousel-slide :name="4" img-src="statics/meetup4.jpeg" />
          <q-carousel-slide :name="5" img-src="statics/meetup5.jpeg" />
          <q-carousel-slide :name="6" img-src="statics/meetup2.jpeg" />
        </q-carousel>
      </div>
    </div>
  </q-page>
</template>

<style>
</style>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      slide: 1
    }
  }
}
</script>
