<template>
  <v-app>
    <v-toolbar app :clipped-left="clipped">
      <v-toolbar-title v-text="title"></v-toolbar-title>
    </v-toolbar>
    <v-content>
      <router-view/>
    </v-content>
    <v-footer :fixed="fixed" app>
      <span>&copy;Prop Edge 2018</span>
    </v-footer>
  </v-app>
</template>

<script>

export default {
  name: 'App',
  data () {
    return {
      clipped: false,
      fixed: false,
      title: 'Prop Edge'
    }
  }
}
</script>
