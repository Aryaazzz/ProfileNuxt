<template>
  <div class="home-wrapper">
    <!-- HERO SECTION -->
    <section class="hero-section">
      <div class="hero-content">
        <div class="badge-blue hero-badge">
          <i class="fas fa-shapes icon-gray"></i>
          <span>Website Profil Resmi Tim</span>
        </div>

        <h1 class="hero-title">
          Sinergi &amp; Dedikasi <br />
          <span class="text-blue">Tim Kelompok 3</span>
        </h1>

        <p class="hero-description">
          Selamat datang di portal profil resmi Kelompok 3. Wadah kolaborasi dan perkenalan anggota tim kami dalam merancang karya teknologi berbasis web yang terstruktur, elegan, dan berdaya guna tinggi.
        </p>

        <div class="hero-actions">
          <a href="#anggota-tim" class="btn-primary">
            <i class="fas fa-users"></i>
            <span>Lihat Anggota Tim</span>
          </a>
          <NuxtLink to="/profil" class="btn-secondary">
            <i class="fas fa-id-card"></i>
            <span>Pelajari Profil Kami</span>
          </NuxtLink>
        </div>
      </div>

      <!-- Quick Metrics Grid -->
      <div class="metrics-grid">
        <div class="metric-card">
          <div class="metric-icon-box">
            <i class="fas fa-users-viewfinder"></i>
          </div>
          <div class="metric-info">
            <span class="metric-number">4</span>
            <span class="metric-label">Anggota Tim Solid</span>
          </div>
        </div>

        <div class="metric-card">
          <div class="metric-icon-box">
            <i class="fas fa-user-shield"></i>
          </div>
          <div class="metric-info">
            <span class="metric-number">1</span>
            <span class="metric-label">Project Manager</span>
          </div>
        </div>

        <div class="metric-card">
          <div class="metric-icon-box">
            <i class="fas fa-laptop-code"></i>
          </div>
          <div class="metric-info">
            <span class="metric-number">3</span>
            <span class="metric-label">Developer Handal</span>
          </div>
        </div>

        <div class="metric-card">
          <div class="metric-icon-box">
            <i class="fas fa-code-branch"></i>
          </div>
          <div class="metric-info">
            <span class="metric-number">100%</span>
            <span class="metric-label">Dedikasi Kolaborasi</span>
          </div>
        </div>
      </div>
    </section>

    <!-- ANGGOTA TIM SHOWCASE -->
    <section id="anggota-tim" class="section-container">
      <div class="section-header">
        <div class="badge-blue">
          <i class="fas fa-users"></i>
          <span>Struktur Tim</span>
        </div>
        <h2 class="section-title">Daftar Anggota &amp; Peran</h2>
        <p class="section-subtitle">
          Susunan struktur kerja Kelompok 3 yang berfokus pada pembagian tugas terencana, keahlian teknis, dan komunikasi efektif.
        </p>
      </div>

      <div class="members-grid">
        <!-- 1. Arya Pamukluhur Prabawa (Project Manager) -->
        <div class="member-card lead-card">
          <div class="card-top">
            <div class="member-avatar-box lead-avatar">
              <span class="avatar-initials">AP</span>
              <div class="role-badge-icon" title="Project Manager">
                <i class="fas fa-crown"></i>
              </div>
            </div>
            <div class="member-status-pill pm-pill">
              <i class="fas fa-circle-dot"></i>
              <span>Project Manager</span>
            </div>
          </div>

          <div class="member-main">
            <h3 class="member-fullname">Arya Pamukluhur Prabawa</h3>
            <span class="member-designation">Ketua Tim &amp; Project Manager</span>
            <p class="member-summary">
              Bertanggung jawab memimpin jalannya proyek, mengkoordinasikan seluruh anggota tim, menetapkan timeline pengerjaan, serta memastikan output sesuai standar kualitas.
            </p>
          </div>

          <div class="member-skills-list">
            <span class="skill-tag"><i class="fas fa-list-check"></i> Project Management</span>
            <span class="skill-tag"><i class="fas fa-users-gear"></i> Team Leadership</span>
            <span class="skill-tag"><i class="fas fa-clipboard-check"></i> Quality Control</span>
          </div>

          <div class="member-card-footer">
            <div class="member-contact-icons">
              <span class="action-icon" title="Profil Lengkap">
                <i class="fas fa-user-tie"></i>
              </span>
              <span class="action-icon" title="Hubungi">
                <i class="fas fa-envelope"></i>
              </span>
              <span class="action-icon" title="Repositori">
                <i class="fas fa-code"></i>
              </span>
            </div>
            <NuxtLink to="/anggota" class="card-detail-link">
              <span>Detail Bio</span>
              <i class="fas fa-arrow-right"></i>
            </NuxtLink>
          </div>
        </div>

        <!-- 2. Alifa Zallfa Nafisa (Developer) -->
        <div class="member-card">
          <div class="card-top">
            <div class="member-avatar-box">
              <span class="avatar-initials">AZ</span>
              <div class="role-badge-icon" title="Developer">
                <i class="fas fa-laptop-code"></i>
              </div>
            </div>
            <div class="member-status-pill dev-pill">
              <i class="fas fa-circle-dot"></i>
              <span>Developer</span>
            </div>
          </div>

          <div class="member-main">
            <h3 class="member-fullname">Alifa Zallfa Nafisa</h3>
            <span class="member-designation">Frontend &amp; Component Developer</span>
            <p class="member-summary">
              Fokus pada pengembangan komponen antarmuka pengguna (UI), integrasi elemen visual yang responsif, dan memastikan kerapian tata letak halaman web.
            </p>
          </div>

          <div class="member-skills-list">
            <span class="skill-tag"><i class="fas fa-code"></i> Vue &amp; Nuxt</span>
            <span class="skill-tag"><i class="fas fa-palette"></i> UI Design System</span>
            <span class="skill-tag"><i class="fas fa-mobile-screen"></i> Responsive</span>
          </div>

          <div class="member-card-footer">
            <div class="member-contact-icons">
              <span class="action-icon" title="Profil Developer">
                <i class="fas fa-terminal"></i>
              </span>
              <span class="action-icon" title="Hubungi">
                <i class="fas fa-envelope"></i>
              </span>
              <span class="action-icon" title="Repositori">
                <i class="fas fa-code"></i>
              </span>
            </div>
            <NuxtLink to="/anggota" class="card-detail-link">
              <span>Detail Bio</span>
              <i class="fas fa-arrow-right"></i>
            </NuxtLink>
          </div>
        </div>

        <!-- 3. M. Afrizal Rinata (Developer) -->
        <div class="member-card">
          <div class="card-top">
            <div class="member-avatar-box">
              <span class="avatar-initials">AR</span>
              <div class="role-badge-icon" title="Developer">
                <i class="fas fa-laptop-code"></i>
              </div>
            </div>
            <div class="member-status-pill dev-pill">
              <i class="fas fa-circle-dot"></i>
              <span>Developer</span>
            </div>
          </div>

          <div class="member-main">
            <h3 class="member-fullname">M. Afrizal Rinata</h3>
            <span class="member-designation">System Logic &amp; Core Developer</span>
            <p class="member-summary">
              Bertanggung jawab atas arsitektur alur data, fungsionalitas komponen, optimasi kinerja peramban, serta penataan struktur berkas proyek.
            </p>
          </div>

          <div class="member-skills-list">
            <span class="skill-tag"><i class="fas fa-gears"></i> Application Logic</span>
            <span class="skill-tag"><i class="fas fa-bolt"></i> Performance</span>
            <span class="skill-tag"><i class="fas fa-sitemap"></i> Data Structure</span>
          </div>

          <div class="member-card-footer">
            <div class="member-contact-icons">
              <span class="action-icon" title="Profil Developer">
                <i class="fas fa-terminal"></i>
              </span>
              <span class="action-icon" title="Hubungi">
                <i class="fas fa-envelope"></i>
              </span>
              <span class="action-icon" title="Repositori">
                <i class="fas fa-code"></i>
              </span>
            </div>
            <NuxtLink to="/anggota" class="card-detail-link">
              <span>Detail Bio</span>
              <i class="fas fa-arrow-right"></i>
            </NuxtLink>
          </div>
        </div>

        <!-- 4. Yeni Dianita (Developer) -->
        <div class="member-card">
          <div class="card-top">
            <div class="member-avatar-box">
              <span class="avatar-initials">YD</span>
              <div class="role-badge-icon" title="Developer">
                <i class="fas fa-laptop-code"></i>
              </div>
            </div>
            <div class="member-status-pill dev-pill">
              <i class="fas fa-circle-dot"></i>
              <span>Developer</span>
            </div>
          </div>

          <div class="member-main">
            <h3 class="member-fullname">Yeni Dianita</h3>
            <span class="member-designation">Layout &amp; Interaction Developer</span>
            <p class="member-summary">
              Bertanggung jawab memastikan kenyamanan interaksi pengguna (UX), standarisasi format tipografi, serta validasi tampilan di ragam resolusi layar.
            </p>
          </div>

          <div class="member-skills-list">
            <span class="skill-tag"><i class="fas fa-pen-ruler"></i> UX Flow</span>
            <span class="skill-tag"><i class="fas fa-cubes-stacked"></i> Modular CSS</span>
            <span class="skill-tag"><i class="fas fa-check-double"></i> Usability</span>
          </div>

          <div class="member-card-footer">
            <div class="member-contact-icons">
              <span class="action-icon" title="Profil Developer">
                <i class="fas fa-terminal"></i>
              </span>
              <span class="action-icon" title="Hubungi">
                <i class="fas fa-envelope"></i>
              </span>
              <span class="action-icon" title="Repositori">
                <i class="fas fa-code"></i>
              </span>
            </div>
            <NuxtLink to="/anggota" class="card-detail-link">
              <span>Detail Bio</span>
              <i class="fas fa-arrow-right"></i>
            </NuxtLink>
          </div>
        </div>
      </div>
    </section>

    <!-- NILAI & PRINSIP KERJA TIM -->
    <section class="section-container">
      <div class="section-header">
        <div class="badge-blue">
          <i class="fas fa-shield-halved"></i>
          <span>Prinsip Kerja</span>
        </div>
        <h2 class="section-title">Nilai Utama Kelompok 3</h2>
        <p class="section-subtitle">
          Pedoman dasar yang mengarahkan setiap langkah tim dalam berkolaborasi dan menyelesaikan setiap tantangan teknis.
        </p>
      </div>

      <div class="values-grid">
        <div class="value-card">
          <div class="value-icon-box">
            <i class="fas fa-handshake"></i>
          </div>
          <h3 class="value-title">Kolaborasi Terbuka</h3>
          <p class="value-desc">
            Setiap anggota tim saling bertukar ide dan saran secara transparan demi mencapai solusi terbaik bersama.
          </p>
        </div>

        <div class="value-card">
          <div class="value-icon-box">
            <i class="fas fa-code-commit"></i>
          </div>
          <h3 class="value-title">Kualitas Kode &amp; Struktur</h3>
          <p class="value-desc">
            Mengedepankan kode yang bersih, mudah dipelihara, dan memiliki standar penamaan komponen yang konsisten.
          </p>
        </div>

        <div class="value-card">
          <div class="value-icon-box">
            <i class="fas fa-bullseye"></i>
          </div>
          <h3 class="value-title">Fokus Solutif &amp; Terarah</h3>
          <p class="value-desc">
            Bekerja sesuai peran dan pembagian modul yang telah ditetapkan oleh Project Manager untuk hasil yang optimal.
          </p>
        </div>
      </div>
    </section>

    <!-- ALUR KERJA TIM (WORKFLOW) -->
    <section class="section-container">
      <div class="section-header">
        <div class="badge-blue">
          <i class="fas fa-timeline"></i>
          <span>Alur Pengembangan</span>
        </div>
        <h2 class="section-title">Tahapan Kolaborasi Proyek</h2>
        <p class="section-subtitle">
          Metodologi bertahap yang kami gunakan dalam membangun website profil ini secara sistematis.
        </p>
      </div>

      <div class="workflow-steps">
        <div class="step-card">
          <div class="step-header">
            <span class="step-number">01</span>
            <div class="step-icon-wrap">
              <i class="fas fa-chart-gantt"></i>
            </div>
          </div>
          <h4 class="step-title">Perencanaan &amp; Inisiasi</h4>
          <p class="step-desc">
            Inisiasi proyek oleh Project Manager (Arya Pamukluhur P.) dengan menentukan spesifikasi, susunan menu, dan aturan warna bersih.
          </p>
        </div>

        <div class="step-card">
          <div class="step-header">
            <span class="step-number">02</span>
            <div class="step-icon-wrap">
              <i class="fas fa-layer-group"></i>
            </div>
          </div>
          <h4 class="step-title">Layout &amp; Sidebar Menu</h4>
          <p class="step-desc">
            Penyusunan arsitektur layout responsif dengan sidebar di sebelah kiri yang memuat menu Home, Profil, Anggota, Kontak, dan Footer.
          </p>
        </div>

        <div class="step-card">
          <div class="step-header">
            <span class="step-number">03</span>
            <div class="step-icon-wrap">
              <i class="fas fa-folder-tree"></i>
            </div>
          </div>
          <h4 class="step-title">Pemisahan Modul Anggota</h4>
          <p class="step-desc">
            Penyediaan berkas halaman mandiri untuk dikembangkan secara independen oleh para Developer (Alifa, Afrizal, Yeni).
          </p>
        </div>

        <div class="step-card">
          <div class="step-header">
            <span class="step-number">04</span>
            <div class="step-icon-wrap">
              <i class="fas fa-circle-check"></i>
            </div>
          </div>
          <h4 class="step-title">Review &amp; Finalisasi</h4>
          <p class="step-desc">
            Pengujian fungsionalitas navigasi, keselarasan warna biru-putih, serta konsistensi tipografi hitam dan abu-abu.
          </p>
        </div>
      </div>
    </section>

    <!-- NAVIGASI CEPAT KE MODUL LAIN (CALL TO ACTION) -->
    <section class="modules-banner">
      <div class="banner-inner">
        <div class="banner-text">
          <div class="badge-blue">
            <i class="fas fa-compass"></i>
            <span>Jelajahi Menu Tim</span>
          </div>
          <h2 class="banner-title">Lanjutkan Eksplorasi Profil Kelompok 3</h2>
          <p class="banner-desc">
            Setiap modul telah disiapkan dalam berkas terpisah untuk dikembangkan oleh rekan-rekan anggota tim secara paralel.
          </p>
        </div>

        <div class="banner-links-grid">
          <NuxtLink to="/profil" class="module-link-card">
            <div class="module-link-icon">
              <i class="fas fa-id-card"></i>
            </div>
            <div class="module-link-info">
              <span class="module-link-title">Halaman Profil</span>
              <span class="module-link-sub">Visi &amp; Misi Tim Kelompok 3</span>
            </div>
            <i class="fas fa-arrow-right module-link-arrow"></i>
          </NuxtLink>

          <NuxtLink to="/anggota" class="module-link-card">
            <div class="module-link-icon">
              <i class="fas fa-users"></i>
            </div>
            <div class="module-link-info">
              <span class="module-link-title">Halaman Anggota</span>
              <span class="module-link-sub">Biodata detail seluruh personil</span>
            </div>
            <i class="fas fa-arrow-right module-link-arrow"></i>
          </NuxtLink>

          <NuxtLink to="/kontak" class="module-link-card">
            <div class="module-link-icon">
              <i class="fas fa-envelope"></i>
            </div>
            <div class="module-link-info">
              <span class="module-link-title">Halaman Kontak</span>
              <span class="module-link-sub">Narahubung &amp; saluran komunikasi</span>
            </div>
            <i class="fas fa-arrow-right module-link-arrow"></i>
          </NuxtLink>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup lang="ts">
useHead({
  title: 'Beranda - Website Profil Kelompok 3'
})
</script>

<style scoped>
.home-wrapper {
  display: flex;
  flex-direction: column;
  gap: 56px;
}

/* =========================================================
   HERO SECTION
   ========================================================= */
.hero-section {
  display: flex;
  flex-direction: column;
  gap: 32px;
  background-color: var(--bg-white);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-lg);
  padding: 40px;
  box-shadow: var(--shadow-sm);
  position: relative;
  overflow: hidden;
}

.hero-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 4px;
  background-color: var(--primary-blue);
}

.hero-content {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 16px;
  max-width: 820px;
}

.hero-badge {
  margin-bottom: 4px;
}

.hero-title {
  font-size: 2.5rem;
  font-weight: 800;
  color: var(--text-black);
  line-height: 1.2;
  letter-spacing: -0.02em;
}

.text-blue {
  color: var(--primary-blue);
}

.hero-description {
  font-size: 1.05rem;
  color: var(--text-gray);
  line-height: 1.7;
}

.hero-actions {
  display: flex;
  align-items: center;
  gap: 14px;
  margin-top: 8px;
  flex-wrap: wrap;
}

/* Metrics Grid */
.metrics-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 16px;
  padding-top: 24px;
  border-top: 1px solid var(--border-light);
}

.metric-card {
  display: flex;
  align-items: center;
  gap: 14px;
  padding: 14px 18px;
  background-color: var(--bg-light);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-md);
  transition: all 0.2s ease;
}

.metric-card:hover {
  background-color: var(--bg-white);
  border-color: var(--primary-blue-subtle);
  transform: translateY(-2px);
  box-shadow: var(--shadow-sm);
}

.metric-icon-box {
  width: 42px;
  height: 42px;
  border-radius: var(--radius-sm);
  background-color: var(--bg-white);
  border: 1px solid var(--border-light);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}

.metric-icon-box i {
  font-size: 1.1rem;
  color: var(--icon-gray);
}

.metric-info {
  display: flex;
  flex-direction: column;
}

.metric-number {
  font-size: 1.35rem;
  font-weight: 800;
  color: var(--text-black);
  line-height: 1.1;
}

.metric-label {
  font-size: 0.78rem;
  color: var(--text-gray);
  font-weight: 500;
}

/* =========================================================
   SECTION HEADERS
   ========================================================= */
.section-container {
  display: flex;
  flex-direction: column;
  gap: 28px;
}

.section-header {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 8px;
}

.section-title {
  font-size: 1.75rem;
  font-weight: 800;
  color: var(--text-black);
  letter-spacing: -0.01em;
}

.section-subtitle {
  font-size: 0.95rem;
  color: var(--text-gray);
  max-width: 680px;
}

/* =========================================================
   MEMBERS GRID
   ========================================================= */
.members-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 24px;
}

.member-card {
  background-color: var(--bg-white);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-lg);
  padding: 24px;
  display: flex;
  flex-direction: column;
  gap: 18px;
  box-shadow: var(--shadow-sm);
  transition: all 0.2s ease;
  position: relative;
}

.member-card:hover {
  border-color: var(--primary-blue-subtle);
  box-shadow: var(--shadow-md);
  transform: translateY(-2px);
}

/* Penekanan khusus untuk Lead Card (Arya Pamukluhur - PM) */
.lead-card {
  border-color: #cbd5e1;
  background: linear-gradient(180deg, #ffffff 0%, #fafbfc 100%);
}

.card-top {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.member-avatar-box {
  width: 54px;
  height: 54px;
  border-radius: var(--radius-md);
  background-color: var(--icon-gray-bg);
  border: 1px solid var(--border-light);
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}

.lead-avatar {
  background-color: var(--primary-blue-light);
  border-color: var(--primary-blue-subtle);
}

.avatar-initials {
  font-size: 1.15rem;
  font-weight: 800;
  color: var(--text-black);
}

.lead-avatar .avatar-initials {
  color: var(--primary-blue);
}

.role-badge-icon {
  position: absolute;
  bottom: -4px;
  right: -4px;
  width: 20px;
  height: 20px;
  border-radius: var(--radius-full);
  background-color: var(--bg-white);
  border: 1px solid var(--border-light);
  display: flex;
  align-items: center;
  justify-content: center;
}

.role-badge-icon i {
  font-size: 0.65rem;
  color: var(--icon-gray);
}

.member-status-pill {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 10px;
  border-radius: var(--radius-full);
  font-size: 0.76rem;
  font-weight: 700;
}

.pm-pill {
  background-color: var(--primary-blue-light);
  color: var(--primary-blue);
  border: 1px solid var(--primary-blue-subtle);
}

.pm-pill i {
  color: var(--primary-blue) !important;
  font-size: 0.5rem;
}

.dev-pill {
  background-color: var(--icon-gray-bg);
  color: var(--text-dark);
  border: 1px solid var(--border-light);
}

.dev-pill i {
  color: var(--icon-gray) !important;
  font-size: 0.5rem;
}

.member-main {
  display: flex;
  flex-direction: column;
  gap: 6px;
}

.member-fullname {
  font-size: 1.2rem;
  font-weight: 800;
  color: var(--text-black);
  letter-spacing: -0.01em;
}

.member-designation {
  font-size: 0.84rem;
  color: var(--text-gray);
  font-weight: 600;
}

.member-summary {
  font-size: 0.88rem;
  color: var(--text-gray);
  line-height: 1.6;
  margin-top: 4px;
}

.member-skills-list {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.skill-tag {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  font-size: 0.74rem;
  color: var(--text-gray);
  background-color: var(--bg-light);
  border: 1px solid var(--border-light);
  padding: 4px 10px;
  border-radius: var(--radius-sm);
  font-weight: 500;
}

.skill-tag i {
  font-size: 0.7rem;
  color: var(--icon-gray);
}

.member-card-footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-top: 14px;
  border-top: 1px solid var(--border-light);
  margin-top: auto;
}

.member-contact-icons {
  display: flex;
  align-items: center;
  gap: 8px;
}

.action-icon {
  width: 30px;
  height: 30px;
  border-radius: var(--radius-sm);
  background-color: var(--bg-light);
  border: 1px solid var(--border-light);
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all 0.15s ease;
}

.action-icon i {
  font-size: 0.78rem;
  color: var(--icon-gray);
}

.action-icon:hover {
  background-color: var(--primary-blue-light);
  border-color: var(--primary-blue-subtle);
}

.action-icon:hover i {
  color: var(--primary-blue);
}

.card-detail-link {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  font-size: 0.82rem;
  font-weight: 600;
  color: var(--primary-blue);
  transition: gap 0.15s ease;
}

.card-detail-link i {
  font-size: 0.75rem;
  color: var(--primary-blue);
}

.card-detail-link:hover {
  gap: 9px;
}

/* =========================================================
   VALUES GRID
   ========================================================= */
.values-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.value-card {
  background-color: var(--bg-white);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-lg);
  padding: 24px;
  display: flex;
  flex-direction: column;
  gap: 12px;
  box-shadow: var(--shadow-sm);
  transition: all 0.2s ease;
}

.value-card:hover {
  border-color: var(--border-subtle);
  transform: translateY(-2px);
  box-shadow: var(--shadow-md);
}

.value-icon-box {
  width: 44px;
  height: 44px;
  border-radius: var(--radius-md);
  background-color: var(--icon-gray-bg);
  border: 1px solid var(--border-light);
  display: flex;
  align-items: center;
  justify-content: center;
}

.value-icon-box i {
  font-size: 1.1rem;
  color: var(--icon-gray);
}

.value-title {
  font-size: 1.05rem;
  font-weight: 700;
  color: var(--text-black);
}

.value-desc {
  font-size: 0.88rem;
  color: var(--text-gray);
  line-height: 1.6;
}

/* =========================================================
   WORKFLOW STEPS
   ========================================================= */
.workflow-steps {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 16px;
}

.step-card {
  background-color: var(--bg-white);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-md);
  padding: 20px;
  display: flex;
  flex-direction: column;
  gap: 10px;
  position: relative;
}

.step-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.step-number {
  font-size: 1.15rem;
  font-weight: 800;
  color: var(--primary-blue);
  background-color: var(--primary-blue-light);
  padding: 2px 10px;
  border-radius: var(--radius-sm);
  border: 1px solid var(--primary-blue-subtle);
}

.step-icon-wrap {
  width: 32px;
  height: 32px;
  border-radius: var(--radius-sm);
  background-color: var(--icon-gray-bg);
  display: flex;
  align-items: center;
  justify-content: center;
}

.step-icon-wrap i {
  font-size: 0.85rem;
  color: var(--icon-gray);
}

.step-title {
  font-size: 0.95rem;
  font-weight: 700;
  color: var(--text-black);
}

.step-desc {
  font-size: 0.82rem;
  color: var(--text-gray);
  line-height: 1.5;
}

/* =========================================================
   MODULES EXPLORATION BANNER
   ========================================================= */
.modules-banner {
  background-color: var(--bg-white);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-lg);
  padding: 36px;
  box-shadow: var(--shadow-sm);
}

.banner-inner {
  display: flex;
  flex-direction: column;
  gap: 24px;
}

.banner-text {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 8px;
}

.banner-title {
  font-size: 1.5rem;
  font-weight: 800;
  color: var(--text-black);
}

.banner-desc {
  font-size: 0.92rem;
  color: var(--text-gray);
}

.banner-links-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
}

.module-link-card {
  display: flex;
  align-items: center;
  gap: 14px;
  padding: 16px;
  background-color: var(--bg-light);
  border: 1px solid var(--border-light);
  border-radius: var(--radius-md);
  transition: all 0.2s ease;
}

.module-link-card:hover {
  background-color: var(--bg-white);
  border-color: var(--primary-blue);
  transform: translateY(-2px);
  box-shadow: var(--shadow-sm);
}

.module-link-icon {
  width: 40px;
  height: 40px;
  border-radius: var(--radius-sm);
  background-color: var(--bg-white);
  border: 1px solid var(--border-light);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}

.module-link-icon i {
  font-size: 1rem;
  color: var(--icon-gray);
}

.module-link-card:hover .module-link-icon i {
  color: var(--primary-blue);
}

.module-link-info {
  display: flex;
  flex-direction: column;
  flex: 1;
}

.module-link-title {
  font-size: 0.92rem;
  font-weight: 700;
  color: var(--text-black);
}

.module-link-sub {
  font-size: 0.76rem;
  color: var(--text-gray);
}

.module-link-arrow {
  font-size: 0.85rem;
  color: var(--text-gray-light);
  transition: transform 0.15s ease, color 0.15s ease;
}

.module-link-card:hover .module-link-arrow {
  transform: translateX(4px);
  color: var(--primary-blue);
}

/* =========================================================
   RESPONSIVE BREAKPOINTS
   ========================================================= */
@media (max-width: 1024px) {
  .metrics-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .members-grid {
    grid-template-columns: 1fr;
  }

  .values-grid {
    grid-template-columns: 1fr;
  }

  .workflow-steps {
    grid-template-columns: repeat(2, 1fr);
  }

  .banner-links-grid {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 640px) {
  .hero-section {
    padding: 24px 18px;
  }

  .hero-title {
    font-size: 1.85rem;
  }

  .metrics-grid {
    grid-template-columns: 1fr;
  }

  .workflow-steps {
    grid-template-columns: 1fr;
  }

  .modules-banner {
    padding: 20px 16px;
  }
}
</style>
