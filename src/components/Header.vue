<template>
  <v-toolbar app>
    <v-toolbar-title class="headline text-uppercase mr-4">
      <span>Stock</span>
      <span class="font-weight-light">Trader</span>
    </v-toolbar-title>
    <v-toolbar-items>
      <v-btn flat to="/">Inicio</v-btn>
      <v-btn flat to="/portfolio">Portfolio</v-btn>
      <v-btn flat to="/stocks">Açoes</v-btn>
    </v-toolbar-items>

    <v-spacer></v-spacer>

    <v-toolbar-items>
      <v-btn flat>Finalizar Dia</v-btn>
      <v-menu offset-y>
        <v-btn flat slot="activator">Salvar & Carregar</v-btn>
        <v-list>
          <v-list-tile>
            <v-list-tile-title>Salvar</v-list-tile-title>
          </v-list-tile>
          <v-list-tile>
            <v-list-tile-title>Carregar</v-list-tile-title>
          </v-list-tile>
        </v-list>
      </v-menu>
    </v-toolbar-items>
  </v-toolbar>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>

</style>