# 📚 Online Kütüphane REST API

Bu proje, bir üniversiteye ait çevrim içi kütüphane sistemine yönelik olarak tasarlanmış bir RESTful API tanımıdır. OpenAPI 3.0.3 spesifikasyonuna uygun şekilde hazırlanmıştır.

## 📌 Projenin Amacı

Bu API, kitapların, öğrencilerin ve ödünç alma işlemlerinin yönetilmesini sağlar. Üniversite kütüphanesi için temel CRUD operasyonlarını kapsayan bir yapı sunar.

## 🛠 Kullanılan Teknolojiler

- OpenAPI Specification 3.0.3
- YAML
- Swagger Editor (test için önerilir)

## 📂 Dosya Yapısı
/
├── openapi.yaml # API tanım dosyası
├── DELIVERY.md # Teslim raporu
└── README.md # Proje açıklaması (bu dosya)


## 🔍 API Özeti

### 🧩 Varlıklar (Entities)

- `books` (Kitaplar)
- `students` (Öğrenciler)
- `loans` (Ödünç alma kayıtları)

### 📌 Temel Endpoint'ler

#### `/books`
- `GET /books` → Tüm kitapları getir (sayfalama destekli)
- `GET /books/{id}` → Belirli bir kitabı getir
- `POST /books` → Yeni kitap ekle
- `PUT /books/{id}` → Kitap bilgilerini güncelle
- `DELETE /books/{id}` → Kitap sil

#### `/students`
- `GET /students`
- `GET /students/{id}`
- `POST /students`
- `PUT /students/{id}`
- `DELETE /students/{id}`

#### `/loans`
- `GET /loans`
- `GET /loans/{id}`
- `POST /loans` → Kitap ödünç alma işlemi
- `PATCH /loans/{id}/return` → Kitap iade işlemi

## 📌 Özellikler

- `components/schemas` ile veri modelleri tanımlandı.
- `parameters` bölümünde query ve path parametreleri kullanıldı.
- `responses` kısmında 200, 201, 400, 404 gibi durumlar örneklerle belirtildi.
- Sayfalama (`page`, `size`) parametreleri `GET /books` için uygulandı.
- Örnek istek ve yanıtlar ile Swagger Editor üzerinden test edilebilir.

## 🧪 Swagger Editor

Projeyi test etmek için [https://editor.swagger.io](https://editor.swagger.io) adresine gidip `openapi.yaml` dosyasını yapıştırabilirsiniz.

## 👤 Geliştirici

- Ad: Kerem Behlül Yeşil
- Öğrenci No: 170422054
- Ders: Açık Kaynak Kodlu Yazılımlar

---
