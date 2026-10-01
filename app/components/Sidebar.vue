<template>
  <aside :class="['sidebar-container', { 'sidebar-open': isOpen }]">
    <!-- Header Brand -->
    <div class="sidebar-brand">
      <div class="brand-logo">
        <i class="fas fa-shapes brand-icon"></i>
      </div>
      <div class="brand-info">
        <span class="brand-title">Kelompok 3</span>
        <span class="brand-subtitle">Project Profile</span>
      </div>
    </div>

    <!-- Navigation Menu -->
    <nav class="sidebar-nav">
      <div class="nav-section-label">MENU UTAMA</div>

      <NuxtLink
        to="/"
        class="nav-link"
        exact-active-class="nav-link-active"
        @click="closeMobileMenu"
      >
        <div class="nav-icon-wrapper">
          <i class="fas fa-house nav-icon"></i>
        </div>
        <span class="nav-text">Home</span>
        <span class="nav-indicator"></span>
      </NuxtLink>

      <NuxtLink
        to="/profil"
        class="nav-link"
        active-class="nav-link-active"
        @click="closeMobileMenu"
      >
        <div class="nav-icon-wrapper">
          <i class="fas fa-id-card nav-icon"></i>
        </div>
        <span class="nav-text">Profil</span>
        <span class="nav-indicator"></span>
      </NuxtLink>

      <NuxtLink
        to="/anggota"
        class="nav-link"
        active-class="nav-link-active"
        @click="closeMobileMenu"
      >
        <div class="nav-icon-wrapper">
          <i class="fas fa-users nav-icon"></i>
        </div>
        <span class="nav-text">Anggota</span>
        <span class="nav-badge">4 Orang</span>
      </NuxtLink>

      <NuxtLink
        to="/kontak"
        class="nav-link"
        active-class="nav-link-active"
        @click="closeMobileMenu"
      >
        <div class="nav-icon-wrapper">
          <i class="fas fa-envelope nav-icon"></i>
        </div>
        <span class="nav-text">Kontak</span>
        <span class="nav-indicator"></span>
      </NuxtLink>

      <div class="nav-divider"></div>

      <div class="nav-section-label">LAINNYA</div>

      <NuxtLink
        to="/footer"
        class="nav-link"
        active-class="nav-link-active"
        @click="closeMobileMenu"
      >
        <div class="nav-icon-wrapper">
          <i class="fas fa-circle-info nav-icon"></i>
        </div>
        <span class="nav-text">Footer & Info</span>
        <span class="nav-indicator"></span>
      </NuxtLink>
    </nav>

    <!-- Sidebar Footer: Info Tim -->
    <div class="sidebar-footer">
      <div class="team-mini-card">
        <div class="team-avatar">
          <i class="fas fa-user-tie member-icon"></i>
        </div>
        <div class="team-details">
          <div class="team-lead-name">Arya Pamukluhur P.</div>
          <div class="team-lead-role">Project Manager</div>
        </div>
      </div>

      <div class="system-status">
        <span class="status-indicator">
          <i class="fas fa-circle status-dot"></i>
          <span class="status-text">Status: Aktif</span>
        </span>
        <span class="version-text">v1.0.0</span>
      </div>
    </div>
  </aside>

  <!-- Overlay untuk Mobile -->
  <div
    v-if="isOpen"
    class="sidebar-backdrop"
    @click="closeMobileMenu"
  ></div>
</template>

<script setup lang="ts">
const props = defineProps<{
  isOpen?: boolean
}>()

const emit = defineEmits<{
  (e: 'close'): void
}>()

const closeMobileMenu = () => {
  emit('close')
}
</script>

<style scoped>
.sidebar-container {
  width: var(--sidebar-width);
  background-color: var(--bg-white);
  border-right: 1px solid var(--border-light);
  height: 100vh;
  position: sticky;
  top: 0;
  display: flex;
  flex-direction: column;
  z-index: 40;
  transition: transform 0.25s ease-in-out;
  flex-shrink: 0;
}

/* Brand Section */
.sidebar-brand {
  height: 72px;
  padding: 0 20px;
  display: flex;
  align-items: center;
  gap: 12px;
  border-bottom: 1px solid var(--border-light);
}

.brand-logo {
  width: 40px;
  height: 40px;
  border-radius: var(--radius-md);
  background-color: var(--primary-blue-light);
  border: 1px solid var(--primary-blue-subtle);
  display: flex;
  align-items: center;
  justify-content: center;
}

.brand-icon {
  font-size: 1.15rem;
  color: var(--primary-blue) !important;
}

.brand-info {
  display: flex;
  flex-direction: column;
}

.brand-title {
  font-size: 1.05rem;
  font-weight: 800;
  color: var(--text-black);
  letter-spacing: -0.01em;
}

.brand-subtitle {
  font-size: 0.75rem;
  font-weight: 500;
  color: var(--text-gray);
}

/* Navigation */
.sidebar-nav {
  flex: 1;
  padding: 20px 14px;
  display: flex;
  flex-direction: column;
  gap: 4px;
  overflow-y: auto;
}

.nav-section-label {
  font-size: 0.7rem;
  font-weight: 700;
  color: var(--text-gray-light);
  letter-spacing: 0.08em;
  padding: 8px 12px 6px;
  text-transform: uppercase;
}

.nav-link {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 14px;
  border-radius: var(--radius-md);
  color: var(--text-dark);
  font-size: 0.92rem;
  font-weight: 600;
  transition: all 0.15s ease;
  position: relative;
}

.nav-icon-wrapper {
  width: 32px;
  height: 32px;
  border-radius: var(--radius-sm);
  background-color: var(--icon-gray-bg);
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.15s ease;
}

.nav-icon {
  font-size: 0.9rem;
  color: var(--icon-gray);
  transition: color 0.15s ease;
}

.nav-text {
  flex: 1;
}

.nav-badge {
  font-size: 0.7rem;
  font-weight: 600;
  padding: 2px 8px;
  border-radius: var(--radius-full);
  background-color: var(--icon-gray-bg);
  color: var(--text-gray);
}

/* Hover State */
.nav-link:hover {
  background-color: var(--bg-light);
  color: var(--text-black);
}

.nav-link:hover .nav-icon-wrapper {
  background-color: var(--border-light);
}

.nav-link:hover .nav-icon {
  color: var(--text-black);
}

/* Active State */
.nav-link-active {
  background-color: var(--primary-blue-light);
  color: var(--primary-blue);
  font-weight: 700;
}

.nav-link-active .nav-icon-wrapper {
  background-color: #ffffff;
  box-shadow: 0 1px 3px rgba(37, 99, 235, 0.15);
}

.nav-link-active .nav-icon {
  color: var(--primary-blue) !important;
}

.nav-link-active .nav-badge {
  background-color: var(--primary-blue);
  color: #ffffff;
}

.nav-divider {
  height: 1px;
  background-color: var(--border-light);
  margin: 14px 6px;
}

/* Sidebar Footer */
.sidebar-footer {
  padding: 16px;
  border-top: 1px solid var(--border-light);
  background-color: #fafbfc;
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.team-mini-card {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 8px 10px;
  background-color: var(--bg-white);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-md);
}

.team-avatar {
  width: 32px;
  height: 32px;
  border-radius: var(--radius-sm);
  background-color: var(--icon-gray-bg);
  display: flex;
  align-items: center;
  justify-content: center;
}

.member-icon {
  font-size: 0.85rem;
  color: var(--icon-gray);
}

.team-details {
  display: flex;
  flex-direction: column;
  overflow: hidden;
}

.team-lead-name {
  font-size: 0.82rem;
  font-weight: 700;
  color: var(--text-black);
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.team-lead-role {
  font-size: 0.72rem;
  color: var(--primary-blue);
  font-weight: 600;
}

.system-status {
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-size: 0.72rem;
  color: var(--text-gray);
  padding: 0 4px;
}

.status-indicator {
  display: flex;
  align-items: center;
  gap: 6px;
}

.status-dot {
  font-size: 0.45rem;
  color: #10b981 !important; /* Hijau status aktif bersih */
}

.version-text {
  font-weight: 600;
  color: var(--text-gray-light);
}

/* Mobile Responsive */
@media (max-width: 900px) {
  .sidebar-container {
    position: fixed;
    top: 0;
    left: 0;
    bottom: 0;
    transform: translateX(-100%);
  }

  .sidebar-container.sidebar-open {
    transform: translateX(0);
    box-shadow: var(--shadow-lg);
  }

  .sidebar-backdrop {
    position: fixed;
    inset: 0;
    background-color: rgba(15, 23, 42, 0.4);
    backdrop-filter: blur(2px);
    z-index: 35;
  }
}
</style>
