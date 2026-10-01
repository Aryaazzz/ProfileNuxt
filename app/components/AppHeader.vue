<template>
  <header class="app-header">
    <div class="header-left">
      <!-- Tombol Hamburger Mobile -->
      <button
        class="mobile-toggle-btn"
        aria-label="Toggle Menu"
        @click="$emit('toggle-sidebar')"
      >
        <i class="fas fa-bars toggle-icon"></i>
      </button>

      <div class="header-breadcrumb">
        <span class="breadcrumb-prefix">Portal Resmi</span>
        <i class="fas fa-chevron-right breadcrumb-separator"></i>
        <span class="breadcrumb-current">{{ currentTitle }}</span>
      </div>
    </div>

    <div class="header-right">
      <div class="header-badge">
        <i class="fas fa-graduation-cap badge-icon"></i>
        <span class="badge-text">Proyek Tim Kelompok 3</span>
      </div>

      <div class="header-date">
        <i class="fas fa-calendar-day date-icon"></i>
        <span>{{ formattedDate }}</span>
      </div>
    </div>
  </header>
</template>

<script setup lang="ts">
import { computed } from 'vue'
import { useRoute } from 'vue-router'

defineEmits<{
  (e: 'toggle-sidebar'): void
}>()

const route = useRoute()

const currentTitle = computed(() => {
  const path = route.path
  if (path === '/') return 'Beranda'
  if (path === '/profil') return 'Profil Tim'
  if (path === '/anggota') return 'Daftar Anggota'
  if (path === '/kontak') return 'Kontak'
  if (path === '/footer') return 'Footer & Informasi'
  return 'Halaman'
})

const formattedDate = computed(() => {
  const now = new Date()
  return new Intl.DateTimeFormat('id-ID', {
    day: 'numeric',
    month: 'short',
    year: 'numeric'
  }).format(now)
})
</script>

<style scoped>
.app-header {
  height: var(--header-height);
  background-color: var(--bg-white);
  border-bottom: 1px solid var(--border-light);
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 32px;
  position: sticky;
  top: 0;
  z-index: 30;
}

.header-left {
  display: flex;
  align-items: center;
  gap: 16px;
}

.mobile-toggle-btn {
  display: none;
  width: 38px;
  height: 38px;
  border-radius: var(--radius-sm);
  background-color: var(--bg-light);
  border: 1px solid var(--border-light);
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all 0.15s ease;
}

.mobile-toggle-btn:hover {
  background-color: var(--border-light);
}

.toggle-icon {
  font-size: 1rem;
  color: var(--icon-gray);
}

.header-breadcrumb {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 0.9rem;
}

.breadcrumb-prefix {
  color: var(--text-gray);
  font-weight: 500;
}

.breadcrumb-separator {
  font-size: 0.65rem;
  color: var(--text-gray-light);
}

.breadcrumb-current {
  color: var(--text-black);
  font-weight: 700;
}

.header-right {
  display: flex;
  align-items: center;
  gap: 16px;
}

.header-badge {
  display: flex;
  align-items: center;
  gap: 8px;
  background-color: var(--primary-blue-light);
  color: var(--primary-blue);
  border: 1px solid var(--primary-blue-subtle);
  padding: 6px 12px;
  border-radius: var(--radius-full);
  font-size: 0.8rem;
  font-weight: 600;
}

.badge-icon {
  font-size: 0.85rem;
  color: var(--primary-blue) !important;
}

.header-date {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 0.82rem;
  color: var(--text-gray);
  padding: 6px 12px;
  background-color: var(--bg-light);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-md);
}

.date-icon {
  font-size: 0.82rem;
  color: var(--icon-gray);
}

@media (max-width: 900px) {
  .app-header {
    padding: 0 16px;
  }

  .mobile-toggle-btn {
    display: flex;
  }

  .header-date {
    display: none;
  }
}
</style>
