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
      <div class="q-pa-md" >
      <q-list dense>
        <q-item>
          <q-item-section>
            <q-item-label>Curso Vue.js</q-item-label>
            <q-item-label caption lines="2">Curso disponibilizado na plataforma Udemy.</q-item-label>
          </q-item-section>

          <q-item-section side top>
            <!-- <q-item-label caption>5 min ago</q-item-label> -->
            <q-btn dense icon="open_in_new" color="green">
              <q-tooltip>
                Visitar Link
              </q-tooltip>
            </q-btn>
            <!-- <q-icon name="star" color="yellow" ></q-icon> -->
          </q-item-section>
        </q-item>

        <q-separator spaced inset ></q-separator>
      </q-list>
    </div>
    </q-tab-panel>

    <q-tab-panel name="cursos">
      <div class="text-h6">Cursos</div>
      Uma lista de cursos
    </q-tab-panel>

    <q-tab-panel name="comunidades">
      <div class="text-h6">Comunidades Locais</div>
      Lista de links de comunidades locais.
    </q-tab-panel>
  </q-tab-panels>
</q-card>

</template>

<script>
export default {
  name: 'Links',
  data () {
    return {
      tab: 'blogs'
    }
  }
}
</script>
