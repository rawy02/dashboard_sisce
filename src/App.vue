<template>
  <v-app class="bg-grey-lighten-8">
    <!-- Paso 3: lo agremos al template -->
    <Navbar />
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
// Pasos para agregar un nuevo componente
// Paso 1: Primero importamos el componete creado en la carpeta componentes
import Navbar from '@/components/Navbar'

export default {
  name: 'App',
  // Paso 2: agregar al componente al export default
  components: {Navbar},
  data () {
    return {
      //
    }
  }
}
</script>