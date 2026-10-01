<template>
  <div class="subpage-container">
    <!-- Header Halaman -->
    <div class="subpage-header">
      <div class="badge-blue">
        <i class="fas fa-users"></i>
        <span>Halaman Anggota</span>
      </div>
      <h1 class="subpage-title">Daftar Anggota Kelompok 3</h1>
      <p class="subpage-desc">
        Halaman detail untuk anggota tim, bio lengkap, keahlian individu, serta portofolio masing-masing personil.
      </p>
    </div>

    <!-- Kotak Panduan untuk Anggota Tim -->
    <div class="card-clean placeholder-box">
      <div class="placeholder-icon-wrap">
        <i class="fas fa-users-gear placeholder-icon"></i>
      </div>
      <h2 class="placeholder-heading">Area Kerja Anggota Tim: Anggota</h2>
      <p class="placeholder-text">
        File ini terletak di <code>app/pages/anggota.vue</code>. Rekan tim dapat mengembangkan profil mendalam untuk Arya, Alifa, Afrizal, dan Yeni di halaman ini.
      </p>
      <div class="placeholder-checklist">
        <div class="check-item">
          <i class="fas fa-check-circle check-icon"></i>
          <span>Biodata Lengkap 4 Anggota</span>
        </div>
        <div class="check-item">
          <i class="fas fa-check-circle check-icon"></i>
          <span>Skill Matrix &amp; Keahlian Teknis</span>
        </div>
        <div class="check-item">
          <i class="fas fa-check-circle check-icon"></i>
          <span>Tautan Portofolio &amp; Media Sosial</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
useHead({
  title: 'Anggota - Kelompok 3'
})
</script>

<style scoped>
.subpage-container {
  display: flex;
  flex-direction: column;
  gap: 24px;
}

.subpage-header {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 8px;
}

.subpage-title {
  font-size: 1.85rem;
  font-weight: 800;
  color: var(--text-black);
}

.subpage-desc {
  font-size: 0.95rem;
  color: var(--text-gray);
  max-width: 650px;
}

.placeholder-box {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding: 48px 24px;
  background-color: var(--bg-white);
  border: 1px dashed var(--border-subtle);
  border-radius: var(--radius-lg);
}

.placeholder-icon-wrap {
  width: 64px;
  height: 64px;
  border-radius: var(--radius-full);
  background-color: var(--icon-gray-bg);
  border: 1px solid var(--border-light);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 16px;
}

.placeholder-icon {
  font-size: 1.6rem;
  color: var(--icon-gray);
}

.placeholder-heading {
  font-size: 1.25rem;
  font-weight: 700;
  color: var(--text-black);
  margin-bottom: 8px;
}

.placeholder-text {
  font-size: 0.9rem;
  color: var(--text-gray);
  max-width: 500px;
  margin-bottom: 24px;
}

.placeholder-text code {
  background-color: var(--icon-gray-bg);
  color: var(--primary-blue);
  padding: 2px 6px;
  border-radius: 4px;
  font-size: 0.85rem;
  font-family: monospace;
}

.placeholder-checklist {
  display: flex;
  flex-direction: column;
  gap: 10px;
  text-align: left;
}

.check-item {
  display: flex;
  align-items: center;
  gap: 10px;
  font-size: 0.88rem;
  color: var(--text-dark);
}

.check-icon {
  font-size: 0.9rem;
  color: var(--icon-gray);
}
</style>
