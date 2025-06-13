---

<div align="center">
  <h1>Lumina Enterprise Solutions</h1>
  <p>
    <i>Menerangi Masa Depan Bisnis dengan Solusi ERP Modern</i>
  </p>
  <p>
    Selamat datang di markas digital kami! Di sinilah kami merancang, membangun, dan menyempurnakan <b>Prism ERP</b>, platform Enterprise Resource Planning berbasis cloud yang dirancang untuk skalabilitas, fleksibilitas, dan efisiensi.
  </p>
</div>

---

## 💎 Tentang Prism ERP

**Prism ERP** bukan sekadar software, melainkan sebuah ekosistem terintegrasi yang memberdayakan bisnis untuk mengelola setiap aspek operasi mereka dengan cerdas. Dibangun di atas arsitektur microservices modern, Prism ERP menawarkan modularitas tak tertandingi, memungkinkan perusahaan untuk mengadopsi fitur yang mereka butuhkan, kapan pun mereka membutuhkannya.

- **Cloud-Native**: Dirancang dari awal untuk berjalan di cloud, memberikan skalabilitas dan keandalan yang luar biasa.
- **Modular**: Dari Keuangan hingga Rantai Pasokan, setiap modul adalah layanan mandiri yang kuat.
- **Developer-Friendly**: Dengan API yang jelas dan dokumentasi yang lengkap, kustomisasi dan integrasi menjadi mudah.

---

## 🚀 Filosofi Kami

Kami percaya pada serangkaian prinsip inti yang memandu setiap baris kode yang kami tulis dan setiap keputusan arsitektur yang kami buat.

| Prinsip | Deskripsi |
| :--- | :--- |
| **Modular by Design** | Kami memecah kompleksitas menjadi layanan-layanan yang terkelola dan independen. Ini memungkinkan tim kami untuk bergerak cepat dan berinovasi tanpa hambatan. |
| **Automation at the Core** | Dari infrastruktur (IaC) hingga CI/CD, kami mengotomatiskan segalanya. Ini membebaskan developer untuk fokus pada apa yang paling penting: menciptakan nilai. |
| **Quality is a Shared Responsibility** | Kualitas bukan hanya tugas Tim QA. Ini adalah budaya yang tertanam dalam proses review kode, pengujian otomatis, dan pemantauan berkelanjutan kami. |
| **Clear Communication & Strong Foundations** | Repositori bersama seperti `prism-api-contracts` dan `prism-common-libs` adalah tulang punggung kami, memastikan konsistensi dan kolaborasi yang efisien di seluruh tim. |

---

## 🗺️ Menavigasi Repositori Kami

Ekosistem kami terorganisir secara logis untuk memudahkan navigasi. Berikut adalah peta repositori utama kami:

| Kategori | Repositori Utama | Deskripsi |
| :--- | :--- | :--- |
| **🏗️ Infrastruktur** | `infra-terraform`, `infra-kubernetes` | Kode sebagai Infrastruktur (IaC) untuk provisioning dan orkestrasi. |
| **⚙️ Layanan Inti** | `prism-auth-service`, `prism-user-service` | Layanan fundamental yang mendukung seluruh platform Prism. |
| **🧩 Modul Backend** | `prism-clarity-backend`, `prism-flow-backend`, dll. | Layanan microservices untuk setiap modul bisnis (Keuangan, SCM, CRM, dll.). |
| **🖥️ Aplikasi Frontend** | `prism-frontend-core`, `prism-frontend-spectrum`, dll. | Antarmuka pengguna berbasis React yang reaktif dan intuitif untuk setiap modul. |
| **📚 Pustaka & Dokumen** | `prism-docs`, `prism-common-libs`, `prism-api-contracts` | Sumber kebenaran untuk dokumentasi, pustaka bersama, dan kontrak API. |
| **🛠️ Perkakas & SDK** | `devtools-cli`, `prism-sdk` | Alat untuk meningkatkan produktivitas developer dan memfasilitasi integrasi. |

---

## 💻 Tumpukan Teknologi Kami

Kami menggunakan teknologi modern dan teruji untuk membangun platform yang andal dan berkinerja tinggi.

<div align="center">
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" alt="Go" />
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes" />
  <img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white" alt="GitHub Actions" />
</div>

---

## 🤝 Cara Kami Bekerja (Panduan Kontribusi)

Konsistensi adalah kunci kolaborasi yang sukses. Semua kontribusi ke dalam ekosistem kami mengikuti alur kerja yang terdefinisi dengan baik.

### 🌿 Alur Kerja Git

Kami menggunakan model branching yang sederhana dan efektif:
- **`main`**: Kode produksi yang stabil. Hanya menerima merge dari branch `release/*`.
- **`develop`**: Cabang integrasi utama untuk fitur-fitur baru.
- **`feature/*`**: Untuk pengembangan fitur baru. Dibuat dari `develop`.
- **`bugfix/*`**: Untuk perbaikan bug non-kritis. Dibuat dari `develop`.
- **`hotfix/*`**: Untuk perbaikan bug kritis di produksi. Dibuat dari `main`.
- **`release/*`**: Untuk mempersiapkan rilis baru (stabilisasi, pengujian akhir). Dibuat dari `develop`.

### ✍️ Format Pesan Commit

Kami menggunakan format *Conventional Commits* untuk pesan commit yang jelas dan terstruktur.

```
[PRISM-123] - feat: tambahkan fitur export CSV ke laporan keuangan

Menambahkan endpoint dan UI untuk memungkinkan pengguna mengekspor data laporan keuangan dalam format CSV.

Closes #456
```

### ✔️ Proses Pull Request (PR)

1.  **Buat PR** dari branch Anda ke `develop` (atau `main` untuk `hotfix`).
2.  **Isi Template PR** dengan deskripsi yang jelas dan tautkan ke tiket Jira terkait.
3.  **Dapatkan Review**: Minimal **2 persetujuan** diperlukan. Code Owner *harus* memberikan persetujuan.
4.  **Lulus CI/CD**: Semua pengujian otomatis harus berhasil dan *code coverage* tidak boleh menurun.
5.  **Merge**: Gunakan "Squash and Merge" untuk menjaga histori `develop` tetap bersih.

---

## ✨ Memulai

Bagi anggota tim baru, langkah pertama Anda adalah:

1.  Dapatkan akses ke repositori yang relevan dengan tim Anda.
2.  Kunjungi repositori [**`prism-docs`**](https://github.com/Lumina-Enterprise-Solutions/prism-docs) untuk panduan onboarding, arsitektur, dan cara menyiapkan lingkungan pengembangan lokal Anda.
3.  Jelajahi repositori [**`devtools-cli`**](https://github.com/Lumina-Enterprise-Solutions/devtools-cli) untuk menginstal alat bantu baris perintah kami yang akan mempermudah hidup Anda.

---

<div align="center">
  <p>Bersama-sama, kita membangun masa depan ERP.</p>
  <p><strong>&copy; Lumina Enterprise Solutions</strong></p>
</div>
