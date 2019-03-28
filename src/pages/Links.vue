<template>
<q-card class="q-pa-md">
  <q-tabs
  v-model="tab"
  dense
  class="text-grey"
  active-color="green"
  indicator-color="green"
  align="justify"
  narrow-indicator
  >
  <q-tab name="blogs" label="Blogs e Artigos" />
  <q-tab name="cursos" label="Cursos" />
  <q-tab name="comunidades" label="Comunidades Locais" />
  </q-tabs>

  <q-tab-panels v-model="tab" animated>
    <q-tab-panel name="blogs">
      <div class="text-h6">Blogs e Artigos</div>
      <blogs></blogs>
    </q-tab-panel>

    <q-tab-panel name="cursos">
      <div class="text-h6">Cursos</div>
      Lista de cursos
    </q-tab-panel>

    <q-tab-panel name="comunidades">
      <div class="text-h6">Comunidades Locais</div>
      <comunidades></comunidades>
    </q-tab-panel>
  </q-tab-panels>
</q-card>

</template>

<script>
import Blogs from 'components/Blogs/Blogs'
import Comunidades from 'components/Comunidades/Comunidades'
export default {
  name: 'Links',
  components: {
    Blogs,
    Comunidades
  },
  data () {
    return {
      tab: 'blogs'
    }
  }
}
</script>
