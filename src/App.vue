<template>
  <div class="flex flex-col h-screen bg-gray-50">
    <!-- Header -->
    <header
      class="flex items-center h-16 px-4 border-b border-gray-300 bg-white shadow-md sm:px-6 lg:px-8"
    >
      <div class="flex items-center">
        <RouterLink class="flex items-center gap-2 font-semibold" to="/">
          <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="40" height="40" />
        </RouterLink>
      </div>
      <nav class="ml-auto space-x-4 flex items-center">
        <RouterLink to="/" class="text-gray-700 hover:text-gray-900">Principal</RouterLink>
        <RouterLink to="/contacto" class="text-gray-700 hover:text-gray-900">Contacto</RouterLink>
        <RouterLink to="/factura" class="text-gray-700 hover:text-gray-900">Factura</RouterLink>
        <RouterLink to="/precio" class="text-gray-700 hover:text-gray-900">Precio</RouterLink>
      </nav>
    </header>
    <!-- Fin Header -->

    <!-- Main -->
    <main class="flex-1 flex items-center justify-center py-6">
      <router-view></router-view>
    </main>
    <!-- Fin Main -->

    <!-- Footer -->
    <footer class="flex items-center h-16 px-4 border-t border-gray-300 bg-white shadow-md">
      <p class="flex-1 text-sm text-gray-600 text-center">
        © MNV Corporation. Todos los derechos reservados
      </p>
    </footer>
    <!-- Fin Footer -->
  </div>
</template>

<script>
import { RouterLink } from 'vue-router'

export default {
  name: 'App',
  components: {
    RouterLink,
  },
}
</script>

<style scoped>
/* Puedes añadir estilos personalizados aquí si es necesario */
</style>
