<template>
  <footer class="app-footer">
    <div class="footer-inner">
      <div class="footer-top">
        <div class="footer-brand-col">
          <div class="footer-logo">
            <div class="footer-logo-box">
              <img src="/logo.png" alt="Logo Kelompok 3" class="footer-brand-img" />
            </div>
            <span class="footer-brand-name">Kelompok 3</span>
          </div>
          <p class="footer-tagline">
            Website profil resmi tim Kelompok 3. Didedikasikan untuk kolaborasi, inovasi, dan pengembangan teknologi web modern.
          </p>
          <div class="footer-social-icons">
            <a href="#" class="social-icon-btn" title="GitHub" aria-label="GitHub">
              <i class="fas fa-code icon-gray"></i>
            </a>
            <a href="#" class="social-icon-btn" title="Email Kontak" aria-label="Email">
              <i class="fas fa-envelope icon-gray"></i>
            </a>
            <a href="#" class="social-icon-btn" title="Dokumentasi Proyek" aria-label="Dokumentasi">
              <i class="fas fa-file-lines icon-gray"></i>
            </a>
          </div>
        </div>

        <div class="footer-links-col">
          <h4 class="footer-heading">Navigasi Utama</h4>
          <ul class="footer-link-list">
            <li><NuxtLink to="/"><i class="fas fa-angle-right link-bullet"></i> Beranda</NuxtLink></li>
            <li><NuxtLink to="/profil"><i class="fas fa-angle-right link-bullet"></i> Profil Tim</NuxtLink></li>
            <li><NuxtLink to="/anggota"><i class="fas fa-angle-right link-bullet"></i> Anggota Kelompok</NuxtLink></li>
            <li><NuxtLink to="/kontak"><i class="fas fa-angle-right link-bullet"></i> Kontak Kami</NuxtLink></li>
          </ul>
        </div>

        <div class="footer-members-col">
          <h4 class="footer-heading">Anggota Tim</h4>
          <ul class="footer-members-list">
            <li>
              <span class="member-name">Arya Pamukluhur P.</span>
              <span class="member-tag pm">Project Manager</span>
            </li>
            <li>
              <span class="member-name">Alifa Zallfa Nafisa</span>
              <span class="member-tag dev">Developer</span>
            </li>
            <li>
              <span class="member-name">M. Afrizal Rinata</span>
              <span class="member-tag dev">Developer</span>
            </li>
            <li>
              <span class="member-name">Yeni Dianita</span>
              <span class="member-tag dev">Developer</span>
            </li>
          </ul>
        </div>
      </div>

      <div class="footer-bottom">
        <p class="copyright-text">
          &copy; {{ currentYear }} Kelompok 3. Seluruh hak cipta dilindungi.
        </p>
        <div class="footer-meta">
          <span class="meta-item">
            <i class="fas fa-shield-halved meta-icon"></i> Nuxt 4 &amp; Vue 3
          </span>
          <span class="meta-item">
            <i class="fas fa-palette meta-icon"></i> Nuansa Biru &amp; Putih
          </span>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup lang="ts">
const currentYear = new Date().getFullYear()
</script>

<style scoped>
.app-footer {
  background-color: var(--bg-white);
  border-top: 1px solid var(--border-light);
  margin-top: auto;
  padding: 40px 32px 24px;
}

.footer-inner {
  max-width: 1280px;
  margin: 0 auto;
}

.footer-top {
  display: grid;
  grid-template-columns: 1.8fr 1fr 1.4fr;
  gap: 36px;
  padding-bottom: 32px;
  border-bottom: 1px solid var(--border-light);
}

.footer-brand-col {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.footer-logo {
  display: flex;
  align-items: center;
  gap: 10px;
}

.footer-logo-box {
  width: 32px;
  height: 32px;
  border-radius: var(--radius-sm);
  background-color: #ffffff;
  border: 1px solid var(--border-light);
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 3px;
  overflow: hidden;
}

.footer-brand-img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.footer-brand-name {
  font-size: 1.15rem;
  font-weight: 800;
  color: var(--text-black);
}

.footer-tagline {
  font-size: 0.88rem;
  color: var(--text-gray);
  line-height: 1.6;
  max-width: 380px;
}

.footer-social-icons {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-top: 4px;
}

.social-icon-btn {
  width: 34px;
  height: 34px;
  border-radius: var(--radius-sm);
  background-color: var(--icon-gray-bg);
  border: 1px solid var(--border-light);
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.15s ease;
}

.social-icon-btn:hover {
  background-color: var(--primary-blue-light);
  border-color: var(--primary-blue-subtle);
}

.social-icon-btn:hover .icon-gray {
  color: var(--primary-blue) !important;
}

.icon-gray {
  font-size: 0.85rem;
  color: var(--icon-gray);
}

.footer-heading {
  font-size: 0.92rem;
  font-weight: 700;
  color: var(--text-black);
  margin-bottom: 14px;
}

.footer-link-list {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.footer-link-list a {
  font-size: 0.88rem;
  color: var(--text-gray);
  display: inline-flex;
  align-items: center;
  gap: 8px;
  transition: color 0.15s ease;
}

.link-bullet {
  font-size: 0.65rem;
  color: var(--text-gray-light);
}

.footer-link-list a:hover {
  color: var(--primary-blue);
}

.footer-members-list {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.footer-members-list li {
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-size: 0.85rem;
}

.member-name {
  color: var(--text-dark);
  font-weight: 500;
}

.member-tag {
  font-size: 0.72rem;
  font-weight: 600;
  padding: 2px 8px;
  border-radius: var(--radius-full);
}

.member-tag.pm {
  background-color: var(--primary-blue-light);
  color: var(--primary-blue);
  border: 1px solid var(--primary-blue-subtle);
}

.member-tag.dev {
  background-color: var(--icon-gray-bg);
  color: var(--text-gray);
}

.footer-bottom {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-top: 20px;
  flex-wrap: wrap;
  gap: 12px;
}

.copyright-text {
  font-size: 0.82rem;
  color: var(--text-gray);
}

.footer-meta {
  display: flex;
  align-items: center;
  gap: 16px;
}

.meta-item {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  font-size: 0.8rem;
  color: var(--text-gray);
}

.meta-icon {
  font-size: 0.75rem;
  color: var(--icon-gray);
}

@media (max-width: 900px) {
  .app-footer {
    padding: 28px 16px 20px;
  }

  .footer-top {
    grid-template-columns: 1fr;
    gap: 24px;
  }

  .footer-bottom {
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>
