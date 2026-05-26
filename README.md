# 📝 Tidy

<p align="center">
  <img src="https://img.shields.io/badge/Expo-000020?style=for-the-badge&logo=expo&logoColor=white" alt="Expo" />
  <img src="https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React Native" />
  <img src="https://img.shields.io/badge/Convex-FF4B4B?style=for-the-badge&logo=convex&logoColor=white" alt="Convex" />
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
</p>

**Tidy** adalah aplikasi manajemen tugas (_Todo List_) berbasis mobile yang dibangun menggunakan **Expo (React Native)** untuk performa mobile yang responsif, serta didukung oleh **Convex** sebagai _backend_ untuk sinkronisasi data secara _real-time_.

Aplikasi ini dibuat sebagai bagian dari pengembangan portofolio proyek _Full-Stack Mobile Development_.

---

## 📂 Struktur Folder

```
├── 📁 app
│   ├── 📁 (tabs)
│   │   ├── 📄 _layout.tsx
│   │   ├── 📄 index.tsx
│   │   └── 📄 settings.tsx
│   └── 📄 _layout.tsx
├── 📁 assets
│   ├── 📁 images
│   │   ├── 🖼️ android-icon-background.png
│   │   ├── 🖼️ android-icon-foreground.png
│   │   ├── 🖼️ icon.png
│   │   └── 🖼️ splash-icon.png
│   └── 📁 styles
│       ├── 📄 home.styles.ts
│       └── 📄 settings.styles.ts
├── 📁 components
│   ├── 📄 DangerZone.tsx
│   ├── 📄 EmptyState.tsx
│   ├── 📄 Header.tsx
│   ├── 📄 LoadingSpinner.tsx
│   ├── 📄 Preferences.tsx
│   ├── 📄 ProgressStats.tsx
│   └── 📄 TodoInput.tsx
├── 📁 convex
│   ├── 📄 schema.ts
│   └── 📄 todos.ts
├── 📁 hooks
│   └── 📄 useTheme.tsx
├── ⚙️ app.json
├── ⚙️ package.json
└── ⚙️ tsconfig.json
```

## ✨ Fitur Utama

- **⚡ Real-time Data Sync:** Semua tugas disinkronkan secara langsung dan instan ke cloud menggunakan Convex backend.
- **🌓 Dynamic Dark & Light Mode:** Dilengkapi dengan `ThemeContext` kustom untuk perpindahan tema yang halus dan nyaman di mata.
- **💾 Persistent Theme Storage:** Pilihan tema pengguna otomatis tersimpan di memori lokal perangkat menggunakan `AsyncStorage`.
- **📱 Native Fluid UI:** Tampilan antarmuka yang bersih, responsif, dan adaptif untuk berbagai ukuran layar Android.

---

## 🛠️ Tech Stack

**Frontend (Mobile App):**

- **Framework:** Expo (React Native) dengan TypeScript
- **Routing:** Expo Router (`_layout` berbasis file)
- **State & Theme Management:** React Context API & UseTheme Hooks
- **Local Storage:** `@react-native-async-storage/async-storage`

**Backend & Database:**

- **Backend platform:** Convex (Deployment Region: US East)
- **Database:** Convex Real-time Document Store

---

## 🚀 Cara Menjalankan Proyek di Lokal

Ikuti langkah-langkah berikut untuk menjalankan proyek **Tidy** di komputer kamu:

### 1. Kloning Repositori

```bash
git clone https://github.com/Aufa18/Tidy.git
cd Tidy
```

### 2. Instalasi Dependensi

Pastikan kamu sudah menginstal [Node.js](https://nodejs.org/) di komputermu. Kemudian, unduh semua _library_ pendukung yang dibutuhkan proyek ini dengan perintah:

```bash
npm install
```

### 3. Konfigurasi Backend & Database (Convex)

Karena Tidy menggunakan Convex untuk sinkronisasi data real-time, kamu harus menghubungkannya ke environment Convex milikmu sendiri. jalankan perintah:

```bash
npx convex dev
```

### 4. Jalankan Aplikasi

Setelah semua persiapan di atas selesai, nyalakan server lokal Expo dengan perintah:

```bash
npx expo start
```
