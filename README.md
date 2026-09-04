# mindmap-manager

# 和心 Wagokoro — Mind Map Manager 🧠

**Wagokoro (和心)** adalah aplikasi **Mind Map Manager berbasis browser** untuk membuat, mengelola, mengorganisir, dan memvisualisasikan ide dalam bentuk node dan koneksi.

Aplikasi ini dibuat menggunakan **HTML, CSS, dan JavaScript** tanpa backend. Data pengguna disimpan secara lokal menggunakan **Browser LocalStorage**, sehingga aplikasi dapat digunakan langsung dari browser.

> 🧠 Turn ideas into structure.

---

## ✨ Features

### 🗂️ Node Management

* ➕ Create new node
* ✏️ Edit node
* 🗑️ Soft delete node
* ♻️ Restore deleted node
* ❌ Permanently delete node
* ☑️ Bulk selection and actions
* 🏷️ Add multiple tags
* 📂 Organize nodes by branch/category
* 📝 Add node descriptions

### 🕸️ Mind Map Canvas

Wagokoro menyediakan visualisasi mind map interaktif.

* Drag & drop nodes
* 🔗 Connect nodes
* ✂️ Remove connections
* 🔍 Zoom in / zoom out
* 🎯 Fit map to view
* ↺ Reset layout
* 🗑️ Clear all connections

Node dan koneksi dapat disimpan sehingga struktur mind map dapat digunakan kembali.

---

## 🔎 Search & Organization

Memudahkan pengguna menemukan dan mengorganisir node:

* 🔍 Search by title
* 🔍 Search by description
* 🔍 Search by tag
* 🏷️ Filter by tag
* 📂 Filter by branch/category
* ↕️ Sort by newest
* ↕️ Sort by oldest
* 🔤 Sort A–Z
* 🔤 Sort Z–A
* 📂 Sort by branch

---

## 🗑️ Trash System

Node yang dihapus tidak langsung hilang.

Wagokoro menggunakan sistem **soft delete**:

```text
Active Node
    ↓
Delete
    ↓
Trash
    ├── Restore
    └── Permanent Delete
```

Dengan sistem ini, pengguna dapat memulihkan node yang tidak sengaja terhapus.

---

## 💾 Local Data Storage

Data aplikasi disimpan menggunakan:

```text
Browser LocalStorage
```

Data yang disimpan mencakup:

* Nodes
* Connections
* Theme
* Save timestamp

Aplikasi secara otomatis menyimpan perubahan ke browser.

> **Note:** Karena menggunakan LocalStorage, data bersifat lokal pada browser/perangkat yang digunakan.

---

## 🔐 Backup & Restore

Wagokoro menyediakan sistem backup dan restore menggunakan JSON.

### Backup

Data dapat diekspor menjadi:

```text
.json
```

### Restore

File JSON yang sebelumnya dibuat dapat dimuat kembali ke aplikasi.

Hal ini berguna untuk:

* Backup data
* Memindahkan data
* Recovery
* Menyimpan snapshot mind map

---

## 📊 Export

Data mind map dapat diekspor ke:

### Excel

```text
.xlsx
```

Data yang diekspor meliputi:

* Judul
* Cabang
* Deskripsi
* Tag
* Tanggal dibuat
* Tanggal diperbarui

### PDF / Print

Aplikasi juga menyediakan fitur **Cetak PDF melalui browser** dengan tabel data mind map.

---

## 🌗 Theme

Tersedia dua tema:

* ☀️ Light Mode
* 🌙 Dark Mode

Pengaturan tema dapat diubah melalui menu Settings.

---

## 🎨 Design

Wagokoro menggunakan desain yang terinspirasi dari estetika Jepang.

Beberapa elemen visual yang digunakan:

* 和心 / Wagokoro branding
* Torii-inspired icon
* Japanese typography
* Indigo
* Vermillion
* Gold
* Paper-like background
* Mind-map visual canvas

Interface menggunakan beberapa font web seperti **Shippori Mincho**, **Yuji Syuku**, dan **Zen Kaku Gothic New**.

---

## 🧩 Technology Stack

| Technology        | Usage                          |
| ----------------- | ------------------------------ |
| HTML5             | Application structure          |
| CSS3              | UI, layout, themes, animations |
| JavaScript        | Application logic              |
| LocalStorage      | Local data persistence         |
| SVG               | Mind map connections & icons   |
| SheetJS           | Excel export                   |
| Browser Print API | PDF / printing                 |

---

## 🚀 Getting Started

Tidak membutuhkan server atau database.

### 1. Clone Repository

```bash
git clone https://github.com/USERNAME/wagokoro-mindmap-manager.git
```

### 2. Masuk ke Directory

```bash
cd wagokoro-mindmap-manager
```

### 3. Jalankan

Buka file:

```text
mindmap-manager.html
```

langsung menggunakan browser.

Atau gunakan local web server:

```bash
python3 -m http.server 8000
```

Kemudian buka:

```text
http://localhost:8000
```

---

## 📁 Project Structure

```text
wagokoro-mindmap-manager/
│
├── mindmap-manager.html
├── README.md
└── LICENSE
```

Aplikasi saat ini dirancang dalam **single HTML file**, sehingga HTML, CSS, dan JavaScript berada dalam satu file utama.

---

## 🧠 Default Mind Map Data

Aplikasi menyediakan beberapa data contoh seperti:

* XMind
* MindMeister
* Scapple
* iThoughts
* Mindnode
* Apa itu Mind Mapping?
* Kriteria Evaluasi

Data tersebut digunakan sebagai initial/demo data ketika belum terdapat data tersimpan di LocalStorage.

---

## 🔒 Privacy

Wagokoro tidak membutuhkan akun atau server backend untuk menyimpan data.

Data utama disimpan pada:

```text
Browser LocalStorage
```

Karena itu:

* Data tidak otomatis tersinkronisasi antar perangkat.
* Menghapus storage browser dapat menghapus data aplikasi.
* Gunakan fitur **Backup JSON** untuk membuat cadangan.

---

## ⚠️ Limitations

Saat ini aplikasi menggunakan penyimpanan lokal sehingga belum menyediakan:

* User authentication
* Cloud synchronization
* Multi-user collaboration
* Online database
* Real-time collaboration

---

## 🛣️ Future Development

Beberapa pengembangan yang dapat ditambahkan:

* [ ] Cloud synchronization
* [ ] Import/export Markdown
* [ ] Import/export JSON yang lebih lengkap
* [ ] PNG/SVG mind map export
* [ ] Keyboard shortcuts
* [ ] Undo / Redo
* [ ] Node hierarchy
* [ ] Custom node colors
* [ ] Custom canvas backgrounds
* [ ] Templates
* [ ] Mobile optimization
* [ ] PWA support
* [ ] Offline installation
* [ ] Cloud database
* [ ] Real-time collaboration

---

## 📜 License

This project is available under the MIT License.

---

## 👤 Author

Created as a lightweight browser-based tool for organizing ideas, research, notes, and knowledge visually.

---

⭐ If you find this project useful, consider giving the repository a **star**.
