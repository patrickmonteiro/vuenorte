<template>
  <div class="q-pa-md" >
    <q-list dense separator>
      <q-item v-for="(blog, index) in blogs" :key="index">
        <q-item-section>
          <q-item-label>{{ blog.titulo }}</q-item-label>
          <q-item-label caption lines="2">
            {{ blog.descricao }}
          </q-item-label>
        </q-item-section>

        <q-item-section side top>
          <q-btn dense
            icon="open_in_new"
            color="green"
            size="sm"
            @click="visitUrl(blog.link)">
            <q-tooltip>
              Visitar Link
            </q-tooltip>
          </q-btn>
        </q-item-section>
      </q-item>
    </q-list>
  </div>
</template>

<script>
import comunidadeData from 'components/Comunidades/comunidades-data'
export default {
  name: 'Comunidades',
  data () {
    return {
      blogs: comunidadeData
    }
  },
  methods: {
    visitUrl (link) {
      window.open(link, '_blank')
    }
  }

}
</script>
