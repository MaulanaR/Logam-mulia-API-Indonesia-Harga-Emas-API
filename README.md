# Emas API ID — API Harga Emas Indonesia

**Emas API ID** adalah layanan **API harga emas Indonesia** yang menyediakan data harga emas dalam format JSON untuk kebutuhan aplikasi, dashboard, website finansial, AI agent, automation, dan integrasi produk digital.

API ini membantu developer mengambil data harga emas dari berbagai brand dan sumber data Indonesia dengan endpoint yang sederhana, ringan, dan mudah digunakan.

> Cocok untuk aplikasi monitoring harga emas, dashboard investasi, chatbot finansial, AI agent, sistem notifikasi harga, website komparasi harga emas, dan otomasi Google Sheets.

---

## SEO Keywords

`API harga emas Indonesia`, `harga emas API`, `API emas Antam`, `API harga Antam`, `API harga UBS`, `API harga Pegadaian`, `API harga Galeri 24`, `gold price API Indonesia`, `harga emas hari ini API`, `JSON harga emas`, `API logam mulia Indonesia`.

---

## Base URL

```txt
https://emas.maulanar.my.id
```

---

## Fitur Utama

* Data harga emas dalam format JSON
* Mendukung berbagai brand dan sumber data emas Indonesia
* Endpoint sederhana dan mudah diintegrasikan
* Tersedia API key untuk penggunaan production
* Support filter, pagination, dan sorting
* Cocok untuk AI agent, dashboard, automation, dan aplikasi finansial

---

## Contoh Penggunaan

### Request

```bash
curl -H "X-API-Key: KUNCI_API_ANDA" \
  "https://emas.maulanar.my.id/api/prices?limit=2"
```

### Contoh Response

```json
{
  "status": "success",
  "data": [
    {
      "brand": "ANTAM",
      "resource": "antam",
      "weight": 1,
      "sell_price": 1574000,
      "buyback_price": 1450000,
      "updated_at": "2026-04-02T10:30:00Z"
    },
    {
      "brand": "UBS",
      "resource": "galeri24",
      "weight": 1,
      "sell_price": 1560000,
      "buyback_price": 1435000,
      "updated_at": "2026-04-02T10:30:00Z"
    }
  ]
}
```

---

## Endpoint Singkat

Beberapa endpoint utama yang tersedia:

```http
GET /api/prices
GET /api/prices/brand/{brand}
GET /api/prices/resource/{resource}
GET /api/prices/today/{brand}
```

Untuk dokumentasi lengkap, parameter, filter, sorting, dan contoh integrasi, silakan lihat:

```txt
https://emas.maulanar.my.id/docs
```

---

## Autentikasi

Gunakan API key pada header request.

### X-API-Key

```bash
curl -H "X-API-Key: KUNCI_API_ANDA" \
  "https://emas.maulanar.my.id/api/prices"
```

### Bearer Token

```bash
curl -H "Authorization: Bearer KUNCI_API_ANDA" \
  "https://emas.maulanar.my.id/api/prices"
```

---

## Brand dan Source

Emas API ID mendukung berbagai brand dan sumber data harga emas Indonesia, seperti:

* ANTAM
* UBS
* Galeri 24
* Pegadaian
* Hartadinata
* King Halim
* Lotus Archi
* Waris Sampoerna

> Brand dan source dapat berbeda. Untuk penggunaan yang lebih presisi, gunakan filter berdasarkan brand dan resource/source.

Detail penggunaan filter tersedia di halaman dokumentasi:

```txt
https://emas.maulanar.my.id/docs
```

---

## Use Case

Emas API ID dapat digunakan untuk:

* Website harga emas hari ini
* Dashboard monitoring harga emas
* Aplikasi investasi emas
* Bot Telegram atau WhatsApp harga emas
* AI agent analisis harga emas
* Automation Google Sheets
* Sistem alert perubahan harga
* Perbandingan harga emas antar source
* Backend aplikasi finansial

---

## Pricing

Emas API ID menyediakan beberapa pilihan paket sesuai kebutuhan, mulai dari testing sampai production.

| Paket      |             Harga |               Kuota | Rate Limit | Cocok Untuk                                |
| ---------- | ----------------: | ------------------: | ---------: | ------------------------------------------ |
| Free       |      Rp 0 / bulan |     60 hits / bulan |      2 RPM | Testing dan validasi endpoint              |
| Lite       | Rp 10.000 / bulan |  1.500 hits / bulan |     10 RPM | MVP dan prototype                          |
| Standard   | Rp 39.000 / bulan |  5.000 hits / bulan |     30 RPM | Aplikasi production skala awal             |
| Pro        | Rp 70.000 / bulan | 20.000 hits / bulan |    100 RPM | AI agent, automation, dan production rutin |

Lihat detail pricing terbaru di:

```txt
https://emas.maulanar.my.id/pricing
```

---

## Dokumentasi Lengkap

Dokumentasi lengkap tersedia di:

```txt
https://emas.maulanar.my.id/docs
```

Di halaman dokumentasi tersedia informasi lebih detail tentang:

* Endpoint API
* Query parameter
* Filter data
* Sorting
* Pagination
* Contoh request
* Contoh response
* Cara menggunakan API key

---

## Status API

```txt
Version: v1.2.1
```

---

## Catatan Penggunaan

Data harga emas dapat berubah mengikuti update dari masing-masing sumber data. Untuk penggunaan production, disarankan untuk:

* Menggunakan API key
* Menyimpan cache sementara
* Menentukan brand dan source secara spesifik
* Menangani response kosong atau error
* Mengikuti batas rate limit sesuai paket

---

## Tentang Emas API ID

Emas API ID dibuat untuk membantu developer, maker, indie hacker, dan pemilik produk digital agar lebih mudah mengintegrasikan data harga emas Indonesia ke dalam aplikasi mereka.

Dengan endpoint JSON yang sederhana, API key, pricing yang jelas, dan dokumentasi yang mudah dipahami, Emas API ID siap digunakan untuk kebutuhan eksperimen, MVP, hingga production.
