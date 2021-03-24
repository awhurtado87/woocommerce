<template>
  <q-layout view="hHh lpR lFf">
    <q-header reveal elevated class="bg-primary text-white">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="left = !left" />

        <q-toolbar-title>
          Control de Tienda
        </q-toolbar-title>
      </q-toolbar>
    </q-header>


      <Menu></Menu>


    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer reveal bordered class="bg-dark text-white">
      <q-toolbar>
        <q-toolbar-title class="text-subtitle1 text-center">
          Gestion de tienda | Todos los derechos reservados
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script>
import Menu from "components/Menu";

export default {
  data() {
    return {
      left: false
    };
  },
  components: {
    Menu
  }
};
</script>
