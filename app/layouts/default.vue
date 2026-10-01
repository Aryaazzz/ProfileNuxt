<template>
  <div class="app-container">
    <!-- Sidebar Kiri -->
    <Sidebar
      :is-open="isSidebarOpen"
      @close="isSidebarOpen = false"
    />

    <!-- Area Konten Utama -->
    <div class="main-viewport">
      <AppHeader
        @toggle-sidebar="isSidebarOpen = !isSidebarOpen"
      />

      <main class="page-content">
        <slot />
      </main>

      <AppFooter />
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import Sidebar from '~/components/Sidebar.vue'
import AppHeader from '~/components/AppHeader.vue'
import AppFooter from '~/components/AppFooter.vue'

const isSidebarOpen = ref(false)
</script>
